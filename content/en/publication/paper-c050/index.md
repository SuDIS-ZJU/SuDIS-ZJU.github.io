---
title: "SpecVLM: Enhancing speculative decoding of video LLMs via verifier-guided token pruning"
authors:
  - "Yicheng Ji"
  - "Jun Zhang"
  - "Heming Xia"
  - "Jinpeng Chen"
  - "Lidan Shou"
  - "Gang Chen"
  - "Huan Li"
author_links:
  - name: "Yicheng Ji"
    url: "/authors/yicheng-ji/home/"
  - name: "Jun Zhang"
    url: "/authors/jun-zhang/home/"
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "The 2025 Conference on Empirical Methods in Natural Language Processing (EMNLP)"
venue: "The 2025 Conference on Empirical Methods in Natural Language Processing (EMNLP)"
publication_kind: "conference"
slug: "paper-c050"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-B"
  - "CORE-A"
abstract: "Video large language models (Vid-LLMs) have shown strong capabilities in understanding video content. However, their reliance on dense video token representations introduces substantial memory and computational overhead in both prefilling and decoding. To mitigate the information loss of recent video token reduction methods and accelerate the decoding stage of Vid-LLMs losslessly, we introduce SPECVLM, a training-free speculative decoding (SD) framework tailored for Vid-LLMs that incorporates staged video token pruning. Building on our novel finding that the draft model’s speculation exhibits low sensitivity to video token pruning, SPECVLM prunes up to 90% of video tokens to enable efficient speculation without sacrificing accuracy. To achieve this, we perform a two-stage pruning process: Stage I selects highly informative tokens guided by attention signals from the verifier (target model), while Stage II prunes the remaining redundant ones in a spatially uniform manner. Extensive experiments on four video understanding benchmarks demonstrate the effectiveness and robustness of SPECVLM, which achieves up to 2.68× decoding speedup for LLaVA-OneVision-72B and 2.11× speedup for Qwen2.5-VL-32B. Code is available at https: //github.com/zju-jiyicheng/SpecVLM."
keywords:
  - "specvlm"
  - "enhancing"
  - "speculative"
  - "decoding"
  - "video"
  - "llms"
  - "verifier"
  - "guided"
doi: "10.18653/v1/2025.emnlp-main.366"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/emnlp/JiZXCSCL25"
  - name: "arXiv"
    url: "https://arxiv.org/abs/2508.16201"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
