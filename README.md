# The Bad Investigator Problem: Multi-Hop Blindness & Competing-Hypothesis Verification Benchmark

**Author:** Taylor Amarel ([papers.baltor.ai](https://papers.baltor.ai) · [blog.baltor.ai](https://blog.baltor.ai) · [notebooks.baltor.ai](https://notebooks.baltor.ai))  
**Monograph PDF:** [`The_Bad_Investigator_Problem_Multi_Hop_Blindness_and_Competing_Hypotheses_2026.pdf`](https://papers.baltor.ai/The_Bad_Investigator_Problem_Multi_Hop_Blindness_and_Competing_Hypotheses_2026.pdf)

## Overview

Why do frontier LLMs and multi-agent swarms perform poorly compared to seasoned human investigators and domain specialists when critical signal is split across **3 to 5 benign-looking hops**?

We observe the exact same structural failure mode across two high-stakes domains:

1. **Counter-Trafficking & Illicit Labor Networks**: A recruitment agency charges a `50,000 PHP` training fee (violating Philippine `RA 10022`), novates the debt to a licensed Hong Kong lender at `68% APR` (violating Hong Kong `Cap. 163`), and ships a contract inside a decorative gift box. Every single document looks ordinary in isolation; the coercion exists strictly in the 3-hop cycle.
2. **Financial Market Alpha vs. Priced-In Consensus**: When asked to evaluate an equity catalyst, unassisted LLMs and homogeneous 5-agent swarms spend **76% to 82% of their token weight** restating public headlines and management guidance already priced into the equity curve, failing to build calibrated probability trees over 2nd- and 3rd-order supply-chain constraints.

## Key Empirical Results

| Architecture | 3-Hop Illicit Structure Recall | Benign Business Precision (`1 - FPR`) | Priced-In Consensus Over-Weighting | Probability Tree Calibration (`1 - Brier`) |
| --- | --- | --- | --- | --- |
| Unassisted Single Frontier LLM | `28.0%` | `68.0%` | `76.0%` (Severe) | `0.31` |
| Homogeneous 5-Agent Swarm (Echo Collapse) | `35.0%` | `62.0%` | `82.0%` (Worse) | `0.29` |
| Naive "Be Suspicious" System Prompt | `66.0%` | `22.0%` (78% False Alarms) | `58.0%` | `0.42` |
| **Typed Multi-Hop Graph + Competing-Hypothesis Verifier** | **`88.0%`** | **`91.0%`** | **`14.0%`** | **`0.88`** |
