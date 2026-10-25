---
title: "HAIL: Hardware Automation through Intelligent Language Models"
excerpt: "A budget-aware LLM agent workflow that repairs and optimizes AMD Vitis HLS C++ kernels using C simulation, synthesis, and C/RTL co-simulation as feedback."
collection: portfolio
permalink: /portfolio/hail/
header:
  teaser: portfolio/thumbs/hail.jpg
---

![HAIL - AI for Hardware Synthesis](/images/portfolio/hail.jpg)

HAIL is a budget-aware agent workflow for repairing and optimizing AMD Vitis HLS C++ kernels. It uses C simulation, synthesis, and C/RTL co-simulation as feedback loops, then grades the resulting kernel for correctness and performance.

**How it works**

1. **Load the contract:** each task supplies kernel code, immutable headers and testbenches, target FPGA part, clock, a credit budget, and an optional co-simulation requirement.
2. **Reach correctness:** C simulation catches compile and functional errors; structural tasks (e.g. DATAFLOW stream deadlocks) additionally require C/RTL co-simulation. Focused log regions are fed back to the model after each failure.
3. **Optimize safely:** correct candidates are synthesized, and optimizations are accepted only if they stay correct and improve measured latency.
4. **Grade independently:** hidden tests, synthesis, and co-simulation run outside the agent budget, producing a correctness-gated score covering latency, resources, tool usage, time, and tokens.

HAIL supports a single-model OpenRouter backend and a CrewAI coder/reviewer backend, plus an optional Qdrant-based hybrid retrieval (RAG) layer that supplies relevant Vitis HLS guidance during optimization. Targets an AMD Alveo U55C with Vitis/Vivado 2025.2.

**Team:** Suraj Karki, Rabigh Khan (Hochschule Bielefeld), Sujan Sharma (TU Dortmund), Muhammad Shaheer (Paderborn University). Advisors: Qazi Arbab Ahmed and Thorsten Jungeblut (Hochschule Bielefeld).

**Tech stack:** Python · LLM Agents · CrewAI · OpenRouter · Qdrant (RAG) · AMD Vitis HLS · Vivado · Docker

[Source code](https://github.com/surajkarki66/HAIL)
