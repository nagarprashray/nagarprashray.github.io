---
title: MESI and MOESI Cache-Coherence Simulator
description: Cycle-accurate C++ simulation of MESI and MOESI coherence across a four-processor shared-memory system.
category: Computer Architecture
organization: Academic project
summary: A trace-driven shared-memory simulator comparing MESI and MOESI coherence behavior under bus contention.
result: MOESI reduced memory-bus traffic by 13% through Owned-state cache-to-cache sharing.
tools:
  - C++
  - MESI
  - MOESI
  - Cache Coherence
  - Cycle-Accurate Simulation
order: 2
---
## Problem

Measure how coherence policy affects bus traffic and transaction behavior in a symmetric multiprocessing system, particularly when dirty cache lines can be supplied by another cache instead of memory.

## What I did

- Developed a cycle-accurate, trace-driven shared-memory simulator for four processors.
- Modeled snooping-based MESI and MOESI finite-state machines in C++.
- Instrumented invalidation behavior, cache-to-cache transfers, memory transactions, and shared-bus arbitration.
- Compared protocol behavior under parallel execution traces and identified contention sources.

## Result

<div class="result-callout">MOESI reduced memory-bus traffic by 13% and lowered transaction latency by using the Owned state for cache-to-cache data sharing.</div>
