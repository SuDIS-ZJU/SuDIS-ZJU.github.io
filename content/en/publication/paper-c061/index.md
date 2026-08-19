---
title: "HARD-KV: Head-Adaptive Regularization for Decoding-time KV Compression"
authors:
  - "Yuxuan Yang"
  - "Feiyang Ren"
  - "Bowen Zeng"
  - "Dalin Zhang"
  - "Jinpeng Chen"
  - "Gang Chen"
  - "Huan Li"
author_links:
  - name: "Yuxuan Yang"
    url: "/authors/yuxuan-yang/home/"
  - name: "Feiyang Ren"
    url: "/authors/feiyang-ren/home/"
  - name: "Bowen Zeng"
    url: "/authors/bowen-zeng/home/"
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2026-01-01"
publishDate: "2026-01-01"
publication_types:
  - "paper-conference"
publication: "The 43th International Conference on Machine Learning (ICML)"
venue: "The 43th International Conference on Machine Learning (ICML)"
publication_kind: "conference"
slug: "paper-c061"
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "Long-context LLM inference faces a fundamental conflict: head-adaptive compression algorithms (e.g., Top-p nucleus sampling) offer superior accuracy by dynamically fluctuating memory budgets, yet modern inference engines (e.g., vLLM) demand rigid, static memory patterns to leverage CUDA Graphs and PagedAttention. We resolve this \"Static-Dynamic\" mismatch with HARD-KV, a unified framework that bridges dynamic selection with rigid system constraints. HARD-KV introduces a Cascade Cache hierarchy, managing the token lifecycle across dense, sparse, and condensed tiers. Crucially, we propose a Logits Calibration mechanism that normalizes diverse importance metrics into a unified probability space, enabling consistent Top-p budgeting across heterogeneous heads. To bridge the efficiency gap, we offer a system-level solution, which rewrites fragmented, dynamic indices into contiguous physical layouts compatible with high-performance inference system. Extensive experiments on math-reasoning benchmarks (AIME, U-Math) verify that HARD-KV achieves up to 2x throughput improvement over static baselines while maintaining high-fidelity generation in 10k+ token scenarios. Code is available at https://github.com/SuDIS-ZJU/HARDInfer."
keywords:
  - "hard"
  - "head"
  - "adaptive"
  - "regularization"
  - "decoding"
  - "time"
  - "compression"
links:
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
