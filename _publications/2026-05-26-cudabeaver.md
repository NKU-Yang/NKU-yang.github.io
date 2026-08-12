---
title: "CUDABeaver: Benchmarking LLM-Based Automated CUDA Debugging"
collection: publications
category: preprints
permalink: /publication/2026-05-26-cudabeaver
excerpt: "CUDABeaver is a benchmark for CUDA debugging built from real failing workspaces produced during LLM-based CUDA generation, evaluating whether a fixer truly repairs failing CUDA code or merely finds a slower test-passing replacement across 213 tasks and seven frontier LLMs."
date: 2026-05-26
venue: "arXiv preprint"
paperurl: "https://arxiv.org/abs/2605.08455"
codeurl: "https://github.com/HaoyangChen23/CUDABeaver"
citation: '<b>S. Li</b>*, H. Chen*, M. Fazzini, C. Ding. &quot;CUDABeaver: Benchmarking LLM-Based Automated CUDA Debugging.&quot; <i>arXiv preprint arXiv:2605.08455</i>, 2026.'
header:
  teaser: "publications/CUDABeaver.png"
---

## Abstract

Debugging CUDA programs has long been challenging because failures often arise from subtle interactions among hardware behavior, compiler decisions, memory hierarchy, and asynchronous execution. Current evaluations of LLM-based CUDA programming largely miss this setting: a model can pass correctness tests with *repair by degeneration*, simplifying the CUDA code into a safer but slower program that abandons the original optimization structure. We introduce **CUDABeaver**, a benchmark for CUDA debugging from real failing workspaces produced during LLM-based CUDA generation. Each task provides the broken candidate, native build/test commands, raw error evidence, and a single editable file. CUDABeaver evaluates whether a fixer truly repairs the failing CUDA code or merely finds a slower test-passing replacement, reporting results by failure category, debugging trajectory, stagnation mode, and performance preservation. We further propose **pass@k(M, C, A)**, a protocol-conditional CUDA debugging metric by making the fixer M, corpus C, and protocol axes A explicit. Using this metric across 213 tasks and seven frontier LLMs, we show that protocol-aware evaluation gives a more faithful view of CUDA debugging ability: when performance-loss tolerance is high, fixers appear much stronger, but even a minor stricter performance requirement can sharply reduce measured success, shifting scores by up to 40 percentage points.

## Key Contributions

- A benchmark of 213 real CUDA debugging tasks harvested from failing workspaces during LLM-based CUDA generation
- Evaluation that distinguishes true repair from "repair by degeneration" into slower test-passing replacements
- The protocol-conditional pass@k(M, C, A) metric, making the fixer, corpus, and protocol axes explicit
- Evaluation of seven frontier LLMs, showing performance requirements can shift scores by up to 40 percentage points

## Authors

**Shiyang Li**\*, Haoyang Chen\*, Mattia Fazzini, Caiwen Ding (\*Equal contribution)

*arXiv preprint arXiv:2605.08455, May 2026.*

![CUDABeaver Benchmark](/images/publications/CUDABeaver.png){: .align-center style="max-width: 100%;"}
