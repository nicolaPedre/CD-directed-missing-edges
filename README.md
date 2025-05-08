# Replication: Infomap Community Detection in Directed Networks

This repository provides a set of Jupyter notebooks for exploring how **Infomap** identifies community structure in **directed networks**, especially in the presence of **disassortativity** and **missing edges**.

The analysis includes both synthetic and empirical datasets, focusing on how Infomap handles directionality and modularity in networks where sources and sinks play a significant role.

---

## Folder: `examples/replication infomap`

This folder contains two key notebooks:

###  1. `Infomap complex SBM.ipynb`

This notebook investigates:
- **Synthetic Stochastic Block Models (SBMs)** with layered source-core-sink structures.
- Effects of **inter- vs. intra-module connectivity**.
- Under what conditions Infomap recovers the original partition.

###  2. `Infomap Empirical Datasets.ipynb`

This notebook applies Infomap to:
- Real-world **directed networks** (e.g., citation graphs, airport networks).
- Compares empirical behavior to predictions from synthetic experiments.
- Examines how **source/sink nodes cluster**, and the role of sparse connections.

---

## 🛠 Requirements

You’ll need the following Python packages:
- `networkx`
- `numpy`
- `matplotlib`
- `infomap` (Python wrapper for the Infomap algorithm)
- `notebook` or `jupyterlab` to run the notebooks

Install all requirements via:

```bash
pip install -r requirements.txt
