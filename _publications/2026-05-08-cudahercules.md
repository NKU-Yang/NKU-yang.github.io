---
title: "CUDAHercules: Benchmarking Hardware-Aware Expert-level CUDA Optimization for LLMs"
collection: publications
category: preprints
permalink: /publication/2026-05-08-cudahercules
excerpt: "CUDAHercules is a benchmark that evaluates LLM-generated CUDA against end-to-end human-expert SOTA systems, spanning single kernels, module-level operators, full applications, and unsolved challenge tasks across Ampere, Hopper, and Blackwell GPUs."
date: 2026-05-08
venue: "arXiv preprint"
paperurl: "https://arxiv.org/abs/2605.08467"
citation: '<b>S. Li</b>, Z. Zhang, G. Sun, Y. Luo, W. Chen, Y. Wang, M. Hong, C. Ding. &quot;CUDAHercules: Benchmarking Hardware-Aware Expert-level CUDA Optimization for LLMs.&quot; <i>arXiv preprint arXiv:2605.08467</i>, 2026.'
header:
  teaser: "publications/CUDAHercules.png"
---

## Abstract

Large language models show promise for automated CUDA programming, however even the strongest coding models may still fall short of expert-level, architecture-aware optimization. We introduce **CUDAHercules**, a benchmark that evaluates generated CUDA against end-to-end human-expert SOTA systems. It spans single kernels, module-level operators, full applications, and unsolved challenge tasks across Ampere, Hopper, and Blackwell GPUs, with end-to-end tasks gated by domain-specific semantic validators. Evaluating frontier models shows a large gap between runnable CUDA and expert CUDA engineering: models often compile and pass tests, but rarely recover the optimization strategies needed to match expert performance. Application semantics further reduce success, and iterative or tool-augmented feedback can improve correctness while drifting toward slow fallback implementations. These results show that automated CUDA programming remains far from fully solved and requires stronger hardware reasoning, better tool use, and training objectives that connect code understanding to hardware architecture-grounded intelligence.

## Key Contributions

- A benchmark evaluating LLM-generated CUDA against end-to-end human-expert SOTA systems
- Coverage of single kernels, module-level operators, full applications, and unsolved challenge tasks across Ampere, Hopper, and Blackwell GPUs
- End-to-end tasks gated by domain-specific semantic validators
- Analysis revealing the gap between runnable CUDA and expert CUDA engineering in frontier models

## Authors

**Shiyang Li**, Zijian Zhang, Guangyan Sun, Yuebo Luo, Winson Chen, Yanzhi Wang, Mingyi Hong, Caiwen Ding

*arXiv preprint arXiv:2605.08467, May 2026.*

![CUDAHercules Benchmark](/images/publications/CUDAHercules.png){: .align-center style="max-width: 100%;"}
