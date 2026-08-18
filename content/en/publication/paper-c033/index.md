---
title: "HyperMR: Efficient hypergraph-enhanced matrix storage on compute-in-memory architecture"
authors:
  - "Yifan Wu"
  - "Ke Chen"
  - "Gang Chen"
  - "Dawei Jiang"
  - "Huan Li"
  - "Lidan Shou"
author_links:
  - name: "Yifan Wu"
    url: "/authors/yifan-wu/home/"
date: "2024-01-01"
publishDate: "2024-01-01"
publication_types:
  - "paper-conference"
publication: "2025 ACM SIGMOD International Conference on Management of Data (SIGMOD)"
slug: "paper-c033"
abstract: "Matrix-vector multiplication (MVM) operations, essential for modern hardware architectures, suffer from heavy I/O overheads and costly serial multiply-add operations. The emerging Compute-in-Memory (CIM) architecture alleviates these issues by enabling in situ MVM operations with O(1) time complexity, eliminating the need to move matrices. However, current storage schemes are still inefficient on CIM due to limited optimization objectives and inflexible support for various access patterns and matrix structures. To address this, we propose HyperMR, a hypergraph-enhanced matrix storage scheme for CIM architectures. First, we identify two performance optimization objectives that are tailored to CIM and prove their NP-hardness. We then introduce a hypergraph modeling approach with a novel access-aware hypergraph generation algorithm to handle diverse matrix structures and access patterns. Moreover, we present a two-phase hypergraph partitioning method to efficiently tackle the NP-hard optimization objectives. Experimental results show that HyperMR outperforms multiple state-of-the-art storage schemes, offering valid optimization for all evaluated matrices, compared to the best-performing baseline which optimizes only 75%. HyperMR also achieves the best average optimization performance for matrix storage layouts, significantly improving efficiency in varied workload scenarios, with a 29.65% improvement on synthetic queries and up to 34.9% on scientific image filtering."
keywords:
  - "hypermr"
  - "efficient"
  - "hypergraph"
  - "enhanced"
  - "matrix"
  - "storage"
  - "compute"
  - "memory"
  - "architecture"
  - "computer science"
doi: "10.1145/3709695"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/pacmmod/WuCCJLS25"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
