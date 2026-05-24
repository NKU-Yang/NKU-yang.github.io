---
title: "StitchCUDA: An Automated Multi-Agents End-to-End GPU Programming Framework with Rubric-based Agentic Reinforcement Learning"
collection: publications
category: conferences
permalink: /publication/2026-03-03-stitchcuda
excerpt: "Accepted to ICML 2026. StitchCUDA is a multi-agent framework for end-to-end GPU program optimization using rubric-based agentic reinforcement learning, achieving ~1.72x speedup over multi-agent baselines and ~2.73x over RL model baselines on KernelBench."
date: 2026-03-03
venue: "International Conference on Machine Learning (ICML 2026)"
paperurl: "https://arxiv.org/abs/2603.02637"
codeurl: "https://github.com/NKU-Yang/StitchCUDA"
header:
  teaser: "publications/stitchCUDA.png"
citation: '<b>S. Li</b>, Z. Zhang, W. Chen, Y. Luo, M. Hong, C. Ding. &quot;StitchCUDA: An Automated Multi-Agents End-to-End GPU Programming Framework with Rubric-based Agentic Reinforcement Learning.&quot; <i>International Conference on Machine Learning (ICML)</i>, 2026.'
---

## Abstract

**Accepted to ICML 2026.**

We propose **StitchCUDA**, an automated multi-agent framework for end-to-end GPU program optimization. The system employs three specialized agents: a Planner coordinating system design, a Coder implementing solutions incrementally, and a Verifier ensuring correctness through performance profiling tools. By incorporating rubric-based agentic reinforcement learning over two atomic skills (code generation and optimization), StitchCUDA prevents reward manipulation and enables advanced CUDA techniques such as kernel fusion.

## Key Results

- Nearly complete success rate on end-to-end GPU tasks
- ~1.72x speedup over multi-agent baselines on KernelBench
- ~2.73x improvement over reinforcement learning model baselines

## Authors

**Shiyang Li**, Zijian Zhang, Winson Chen, Yuebo Luo, Mingyi Hong, Caiwen Ding
