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
    url: "/authors/bowen-zeng/home/zh/"
  - name: "Feiyang Ren"
    url: "/authors/feiyang-ren/home/zh/"
  - name: "Jun Zhang"
    url: "/authors/jun-zhang/home/zh/"
  - name: "Huan Li"
    url: "/authors/huan-li/home/zh/"
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
abstract: "movements. [cs.AI] 7 Apr 2026 Visual Tokens Text Tokens Text-guided Classification Multimodal Large Language Models (MLLMs) Attention Static Heads Dynamic Heads Head Type w. Static Pruning w. Dynamic Retrieval have advanced unified reasoning over text, im- KV Cache ages, and videos, but their inference is hin- Budget dered by the rapid growth of key-value (KV) caches. Each visual input expands into thou- sands of tokens, causing caches to scale lin- Figure 1: Left: We introduce H YBRID KV, a hybrid KV early with context length and remain resident cache compression framework for efficient yet effective in GPU memory throughout decoding, which MLLM inference. H YBRID KV leverages head-level at- leads to prohibitive memory overhead and la- tention patterns (detailed in Section 2) to classify static tency even on high-end GPUs. A common so- and dynamic heads via text-guided signals, enabling lution is to compress caches under a fixed allo- hierarchical budget allocation with tailored pruning and cated budget at different granularities: token- retrieval strategies. Right: H YBRID KV outperforms level uniformly discards less important tokens, existing counterparts including S NAP KV (Li et al., layer-level varies retention across layers, and 2024b), LOOK-M (Wan et al., 2024), M ADA KV (Li head-level redistributes budgets across heads. et al., 2025) and S PARSE MM (Wang et al., 2025) on Yet these approaches stop at allocation and eight benchmarks using only 10% of the KV cache on overlook the heterogeneous behaviors of at- Qwen2.5-VL-7B. Performance metrics are shown as a tention heads that require distinct compres- percentage relative to F ULL C ACHE. sion strategies. We propose H YBRID KV, a hybrid KV cache compression framework that integrates complementary strategies in three stages: heads are first classified into static or language and visual modalities. To support such dynamic types using text-centric attention; then capability, they process long multimodal contexts a top-down budget allocation scheme hierar- in which each high-resolution image or video chically assigns KV budgets; finally, static frame unfolds into hundreds of tokens, rapidly heads are compressed by text-prior pruning inflating sequence lengths. This expansion directly and dynamic heads by chunk-wise retrieval. drives a linear growth of Key-Value (KV) caches, Experiments on 11 multimodal benchmarks which store the key and value representations of with Qwen2.5-VL-7B show that H YBRID KV reduces KV cache memory by up to 7.9× and all past tokens for attention computation and must achieves 1.52× faster decoding, with almost be retained throughout autoregressive decoding. no performance drop or even higher relative to For instance, a 72B-scale Qwen2.5-VL processing the full-cache MLLM. 20 images already exceeds 40K tokens and 13 GB of cache, while a 5-second 720p video surpasses"
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
