# IPMQ-Sim

IPMQ-Sim is a Discrete-Event Simulation (DES) framework built on SimPy for generating multivariate synthetic datasets with operational coherence via explicit coupling of the Production–Maintenance–Quality (PMQ) triad.  
The primary Machine Learning target is Remaining Useful Life (RUL) prediction, with per-asset episode labeling generated directly from simulated run-to-failure trajectories.

---

## Motivation

Industrial ML research is frequently constrained by limited access to high-quality historical data, particularly for rare failures and extreme operating regimes. Furthermore, industrial privacy and intellectual property restrictions hinder cross-organization data sharing. IPMQ-Sim addresses this gap by producing synthetic time-series datasets where degradation and quality outcomes emerge from a causal operational mechanism rather than from context-blind stochastic drift.

---

## Core Contributions

- **Operational coherence (PMQ coupling):** load → degradation → quality risk.
- **DES-first architecture:** process-level concurrency and asynchronous behavior modeled through SimPy.
- **Multi-archetype physics:** rotary / tooling / thermal / electronic behavior families.
- **Reproducibility:** deterministic experiments via global seed and independent per-machine RNG streams.
- **Supervised learning readiness:** consolidated tabular dataset with **RUL labels** per machine episode.
- **Maintenance (optional):** minimal intervention events (downtime + partial wear reset) to explicitly represent “M” in PMQ.

---

## Repository Layout

