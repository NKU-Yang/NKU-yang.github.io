---
title: "SparseDitto: Customizing GPU Kernels for Different Sparsity Patterns with LLM-Based Agentic System"
collection: publications
category: preprints
permalink: /publication/2026-08-12-sparseditto
excerpt: "SparseDitto is an LLM-based agentic system that constructs a customized GPU kernel for each matrix, operator, and target GPU, supporting SpMV, SpMM, and SpGEMM, achieving a geometric-mean speedup of 2.68x over cuSPARSE on an RTX PRO 6000 and 2.79x on an H200."
date: 2026-08-12
venue: "arXiv preprint"
paperurl: "https://arxiv.org/abs/2608.05033"
citation: '<b>S. Li</b>, G. Sun, J. Tang, Y. Wang, M. Hong, C. Ding. &quot;SparseDitto: Customizing GPU Kernels for Different Sparsity Patterns with LLM-Based Agentic System.&quot; <i>arXiv preprint arXiv:2608.05033</i>, 2026.'
header:
  teaser: "publications/SparseDitto.png"
---

## Abstract

Sparse matrix kernels are fundamental to scientific computing, graph analytics, and machine learning. Their GPU performance depends strongly on the input sparsity pattern and execution strategy. For the same SpMM on the same matrix, cuSPARSE exhibits a 350x performance gap between CSR and Blocked-ELL. Our study of multiple data formats, specialized systems, and sparse compilers shows that no single implementation consistently dominates across sparsity patterns and operators. This motivates a system that can adapt its representation, execution strategy, and hardware mapping to each workload and target GPU. We present **SparseDitto**, an LLM-based system that constructs a GPU kernel for each matrix, operator, and target GPU. SparseDitto supports SpMV, SpMM, and SpGEMM within a unified design framework. A lightweight additive model ranks established strategies using structural features of the input matrix. An architecture-aware planner then proposes several candidate designs. Coding and verification agents implement and refine them using measurements from the target GPU. Across three sparse operators and a diverse set of matrices, SparseDitto achieves a geometric-mean speedup of 2.68x over cuSPARSE on an NVIDIA RTX PRO 6000 GPU, with a maximum of 146.61x. On an NVIDIA H200 GPU, it achieves 2.79x, with a maximum of 78.5x. Its generated SpMM kernels also accelerate full-batch GCN training by up to 3.39x.

## Key Contributions

- An LLM-based agentic system that customizes GPU kernels per matrix, operator, and target GPU
- Unified support for SpMV, SpMM, and SpGEMM with a lightweight additive model ranking strategies from structural matrix features
- Architecture-aware planning with coding and verification agents refined by on-device measurements
- Geometric-mean speedups of 2.68x (RTX PRO 6000) and 2.79x (H200) over cuSPARSE, and up to 3.39x faster full-batch GCN training

## Authors

**Shiyang Li**, Guangyan Sun, Jinwei Tang, Yanzhi Wang, Mingyi Hong, Caiwen Ding

*arXiv preprint arXiv:2608.05033, August 2026.*

![SparseDitto System](/images/publications/SparseDitto.png){: .align-center style="max-width: 100%;"}
