---
title: I2C Multi-Bus Verification Using Layered UVM
description: Layered SystemVerilog UVM verification of a configurable I2C multi-bus controller with coverage-driven regressions.
category: Design Verification
organization: Academic project
summary: A layered UVM environment for a configurable I2C multi-bus controller with Avalon-MM and Wishbone host interfaces.
result: 92% functional coverage with assertion-linked coverage analysis.
tools:
  - SystemVerilog
  - UVM
  - SVA
  - VHDL
  - I2C
order: 1
---
## Problem

Verify a configurable I2C Multi-Bus master controller across its host-side register interfaces and multi-master, multi-bus behavior. The environment needed reusable components, protocol-aware checking, and coverage feedback rather than a collection of directed tests.

## What I did

- Designed the controller integration around VHDL RTL with Avalon-MM and Wishbone interfaces for SoC use.
- Built layered SystemVerilog UVM agents, sequencers, drivers, monitors, and a scoreboard.
- Exercised multi-master and multi-bus behavior through modular sequences and automated regressions.
- Connected assertions and functional coverage to expose missing protocol and configuration scenarios.

## Result

<div class="result-callout">Reached 92% functional coverage through automated regression and assertion-linked coverage analysis.</div>
