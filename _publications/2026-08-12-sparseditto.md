---
title: "SparseDitto: An Agentic Sparse Compilation Framework through Architecture-Aware Synthesis on GPUs"
collection: publications
category: preprints
permalink: /publication/2026-08-12-sparseditto
excerpt: "SparseDitto is an agentic sparse compilation framework for sparse matrix computation on GPUs that jointly synthesizes representation, execution schedule, and hardware mapping in a unified compilation plan. It covers SpMV, SpMM, and SpGEMM and achieves geometric-mean speedups over cuSPARSE of 2.68x on an RTX PRO 6000 and 2.79x on an H200."
date: 2026-08-12
venue: "arXiv preprint"
paperurl: "https://arxiv.org/abs/2608.05033"
citation: '<b>S. Li</b>, G. Sun, J. Tang, Y. Wang, M. Hong, C. Ding. &quot;SparseDitto: An Agentic Sparse Compilation Framework through Architecture-Aware Synthesis on GPUs.&quot; <i>arXiv preprint arXiv:2608.05033</i>, 2026.'
header:
  teaser: "publications/SparseDitto.png"
---

## Abstract

Sparse matrix computation performance on GPU depends on how representation and execution schedule match the input structure and target hardware. No single implementation consistently dominates across sparsity patterns, operators, and hardwares. Existing sparse compilers and specialized systems cannot cover all of them simultaneously. We present **SparseDitto**, an agentic sparse compilation framework for sparse matrix computation on GPUs. It jointly synthesizes representation, execution schedule, and hardware mapping in a unified compilation plan. Structural analysis and a learned template-ranking prior guide architecture-aware synthesis. LLM-guided lowering realizes each plan as CUDA code, while target-GPU profiling drives plan refinement. SparseDitto covers multiple operators, e.g., SpMV, SpMM, and SpGEMM, and various representations within one framework. It can also automatically adapt to different hardwares. Across various SuiteSparse matrices, SparseDitto achieves geometric-mean speedups over cuSPARSE of 2.68x on an NVIDIA RTX PRO 6000 and 2.79x on an NVIDIA H200 (up to 146.61x). Its generated SpMM kernels accelerate full-batch GCN training by up to 3.39x.

## Key Contributions

- An agentic sparse compilation framework that jointly synthesizes representation, execution schedule, and hardware mapping in a unified compilation plan
- Architecture-aware synthesis guided by structural analysis and a learned template-ranking prior
- LLM-guided lowering of each plan to CUDA code, with target-GPU profiling driving plan refinement
- Unified coverage of SpMV, SpMM, and SpGEMM across multiple representations, with automatic adaptation to different GPUs
- Geometric-mean speedups over cuSPARSE of 2.68x (RTX PRO 6000) and 2.79x (H200), up to 146.61x, and up to 3.39x faster full-batch GCN training

## Authors

**Shiyang Li**, Guangyan Sun, Jinwei Tang, Yanzhi Wang, Mingyi Hong, Caiwen Ding

*arXiv preprint arXiv:2608.05033, August 2026.*

![SparseDitto System](/images/publications/SparseDitto.png){: .align-center style="max-width: 100%;"}
