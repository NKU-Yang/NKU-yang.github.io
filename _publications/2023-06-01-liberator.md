---
title: "Liberator: A Data Reuse Framework for Out-of-Memory Graph Computing on GPUs"
collection: publications
category: manuscripts
permalink: /publication/2023-06-01-liberator
excerpt: "Liberator is a data reuse framework that enables efficient out-of-memory graph computing on GPUs by intelligently managing data transfers between host and device memory."
date: 2023-06-01
venue: "IEEE Transactions on Parallel and Distributed Systems (TPDS)"
paperurl: "https://ieeexplore.ieee.org/abstract/document/10107428"
citation: '<b>S. Li</b>, R. Tang, J. Zhu, Z. Zhao, X. Gong, W. Wang, J. Zhang, P.-C. Yew. &quot;Liberator: A Data Reuse Framework for Out-of-Memory Graph Computing on GPUs.&quot; <i>IEEE Transactions on Parallel and Distributed Systems (TPDS)</i>, 34(6): 1954-1967, 2023.'
header:
  teaser: "publications/liberator.png"
---

## Abstract

We present **Liberator**, a data reuse framework that enables efficient out-of-memory graph computing on GPUs. When graph data exceeds GPU memory capacity, Liberator intelligently partitions graph data and schedules computation to maximize data reuse across partitions, significantly reducing the overhead of CPU-GPU data transfers.

## Key Contributions

- A novel data reuse framework for out-of-memory graph processing on GPUs
- Intelligent graph partitioning and scheduling to minimize data transfer overhead
- Demonstrated significant speedups over existing out-of-memory GPU graph frameworks

## Authors

**Shiyang Li**, Ruiqi Tang, Jingyu Zhu, Ziyi Zhao, Xiaoli Gong, Wenwen Wang, Jin Zhang, Pen-Chung Yew

*IEEE Transactions on Parallel and Distributed Systems (TPDS)*, 34(6): 1954-1967, 2023.

![Liberator Framework](/images/publications/liberator.png){: .align-center style="max-width: 100%;"}
