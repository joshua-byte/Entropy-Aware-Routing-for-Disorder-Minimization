# Entropy-Aware Routing for Disorder Minimization

## Overview
This project implements an entropy-aware routing framework designed to improve network stability under dynamic and adversarial conditions such as DDoS attacks.

Traditional routing methods (e.g., shortest-path) optimize only for distance, ignoring variability in traffic. This project introduces an entropy-based metric that captures traffic instability and uses it to guide routing decisions.

---

## Key Idea
Routing is reformulated as a **disorder-aware optimization problem**, where paths are selected to minimize cumulative entropy rather than just hop count.

- High variance in traffic → high entropy → unstable edge  
- Low variance → low entropy → stable edge  

---

## Features
- Entropy-based edge weighting using traffic variance
- Simulation of dynamic network traffic
- Distributed DDoS-style attack injection
- Comparison between:
  - Shortest-path routing
  - Entropy-aware routing
- Metrics evaluated:
  - Path length
  - Cumulative entropy
  - Attack exposure

---

## Dataset
- Link to the Dataset (https://snap.stanford.edu/data/ego-Twitter.html)
- Twitter social network graph
- ~81,000 nodes and ~1.3M edges
- Sampled subgraph used for efficiency (~15,000 nodes)

## Source Citation
J. McAuley and J. Leskovec. Learning to Discover Social Circles in Ego Networks. NIPS, 2012
