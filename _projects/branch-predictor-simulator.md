---
title: Branch-Predictor Simulator for Execution-Trace Analysis
description: C++ simulator comparing bimodal, gshare, and hybrid branch-prediction algorithms using processor traces.
category: Computer Architecture
organization: Academic project
summary: A configurable C++ simulator for evaluating bimodal, gshare, and tournament branch predictors on execution traces.
result: Achieved 90% prediction accuracy and a one-percentage-point gain over the bimodal baseline.
tools:
  - C++
  - Bimodal
  - Gshare
  - Hybrid Predictor
  - Trace Simulation
order: 3
---
## Problem

Evaluate branch-prediction organizations and parameter choices that reduce mispredictions and pipeline flushes in a speculative superscalar processor.

## What I did

- Built a configurable C++ simulator for bimodal, gshare, and tournament/hybrid prediction.
- Implemented pattern-history-table indexing, global-history updates, selector training, and predictor statistics.
- Swept predictor configurations against processor execution traces to compare accuracy and storage tradeoffs.
- Analyzed how history length and table sizing affected simulated pipeline stalls.

## Result

<div class="result-callout">Reached 90% prediction accuracy, improving by one percentage point over the bimodal baseline and reducing simulated pipeline stalls.</div>
