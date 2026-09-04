---
title: "PagePilot: Synergizing Heterogeneous Backend Devices with Reusability-Aware Page Offloading"
collection: publications
category: manuscripts
permalink: /publication/2026-09-03-pagepilot
excerpt: "PagePilot is a reuse-aware page offloading framework for heterogeneous swap systems that tracks refault behavior and guides backend placement, reducing page-fault handler latency by 10.8% and increasing fast-device utilization by 51.8% under memory pressure."
date: 2026-09-03
venue: "ACM Transactions on Architecture and Code Optimization (TACO)"
paperurl: "/files/pagepilot.pdf"
codeurl: "https://github.com/NKU-EmbeddedSystem/pagepilot"
citation: 'X. Liu, J. Dong, X. Liu, L. Wang, <b>S. Li</b>, H. Li, X. Gong, J. Zhang, P.-C. Yew. &quot;PagePilot: Synergizing Heterogeneous Backend Devices with Reusability-Aware Page Offloading.&quot; <i>ACM Transactions on Architecture and Code Optimization (TACO)</i>, 2026. doi:10.1145/3845616.'
header:
  teaser: "publications/pagepilot.png"
  teaser_side: true
---

## Abstract

Page swapping remains the dominant mechanism for extending physical memory, but Linux swap management still relies on priority-based backend selection when heterogeneous devices are available. This can leave fast devices occupied by rarely reused pages while frequently refaulted pages are placed on slower devices. We present **PagePilot**, a reuse-aware page offloading framework for heterogeneous swap systems. PagePilot tracks refault behavior across eviction and refault cycles, uses average refault distance to guide backend selection, and applies background migration to correct misplacements. Implemented in the Linux 6.3 kernel, PagePilot reduces page-fault handler latency by 10.8%, increases fast-device utilization by 51.8%, and outperforms iSwap in 37 of 40 evaluated configurations.

## Key Contributions

- A reuse-aware page offloading framework for heterogeneous swap backends
- Refault-history tracking that bridges virtual memory semantics and swap backend placement
- Background migration that preserves fast-device capacity for pages with imminent reuse
- Linux 6.3 kernel implementation with lower page-fault latency and higher fast-backend utilization

## Authors

Xingze Liu, Jialin Dong, Xinyu Liu, Lizhi Wang, **Shiyang Li**, Haoran Li, Xiaoli Gong, Jin Zhang, Pen-Chung Yew

*ACM Transactions on Architecture and Code Optimization (TACO), 2026. doi:10.1145/3845616.*

![PagePilot Overview](/images/publications/pagepilot.png){: .align-center style="max-width: 100%;"}
