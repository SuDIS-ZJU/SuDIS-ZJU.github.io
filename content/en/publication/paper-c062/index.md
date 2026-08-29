---
title: "HybridKV: Hybrid KV Cache Compression for Efficient Multimodal Large Language Model Inference"
authors:
  - "Bowen Zeng"
  - "Feiyang Ren"
  - "Jun Zhang"
  - "Xiaoling Gu"
  - "Ke Chen"
  - "Lidan Shou"
  - "Huan Li"
author_links:
  - name: "Bowen Zeng"
    url: "/authors/bowen-zeng/home/"
  - name: "Feiyang Ren"
    url: "/authors/feiyang-ren/home/"
  - name: "Jun Zhang"
    url: "/authors/jun-zhang/home/"
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2026-01-01"
publishDate: "2026-01-01"
publication_types:
  - "paper-conference"
publication: "The 64th Annual Meeting of the Association for Computational Linguistics (ACL)"
venue: "The 64th Annual Meeting of the Association for Computational Linguistics (ACL)"
publication_kind: "conference"
slug: "paper-c062"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "Multimodal Large Language Models (MLLMs) have advanced unified reasoning over text, images, and videos, but their inference is hindered by the rapid growth of key-value (KV) caches. Each visual input expands into thousands of tokens, causing caches to scale linearly with context length and remain resident in GPU memory throughout decoding, which leads to prohibitive memory overhead and latency even on high-end GPUs. A common solution is to compress caches under a fixed allocated budget at different granularities: tokenlevel uniformly discards less important tokens, layer-level varies retention across layers, and head-level redistributes budgets across heads. Yet these approaches stop at allocation and overlook the heterogeneous behaviors of attention heads that require distinct compression strategies. We propose HYBRIDKV, a hybrid KV cache compression framework that integrates complementary strategies in three stages: heads are first classified into static or dynamic types using text-centric attention; then a top-down budget allocation scheme hierarchically assigns KV budgets; finally, static heads are compressed by text-prior pruning and dynamic heads by chunk-wise retrieval. Experiments on 11 multimodal benchmarks with Qwen2.5-VL-7B show that HYBRIDKV reduces KV cache memory by up to 7.9× and achieves 1.52× faster decoding, with almost no performance drop or even higher relative to the full-cache MLLM."
keywords:
  - "hybridkv"
  - "hybrid"
  - "cache"
  - "compression"
  - "efficient"
  - "multimodal"
  - "large"
  - "language"
doi: "10.48550/arxiv.2604.05887"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/corr/abs-2604-05887"
  - name: "arXiv"
    url: "https://arxiv.org/abs/2604.05887"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
