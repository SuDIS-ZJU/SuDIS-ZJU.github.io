---
title: "See the Forest for the Trees: Loosely Speculative Decoding via Visual-Semantic Guidance for Efficient Inference of Video LLMs"
authors:
  - "Yicheng Ji"
  - "Jun Zhang"
  - "Jinpeng Chen"
  - "Cong Wang"
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
date: "2026-01-01"
publishDate: "2026-01-01"
publication_types:
  - "paper-conference"
publication: "The 64th Annual Meeting of the Association for Computational Linguistics (ACL)"
venue: "The 64th Annual Meeting of the Association for Computational Linguistics (ACL)"
publication_kind: "conference"
slug: "paper-c068"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "Video Large Language Models (Video-LLMs) excel in video understanding but suffer from high inference latency during autoregressive generation. Speculative Decoding (SD) mitigates this by applying a draft-and-verify paradigm, yet existing methods are constrained by rigid exact-match rules, severely limiting the acceleration potential. To bridge this gap, we propose LVSPEC, the first trainingfree loosely SD framework tailored for VideoLLMs. Grounded in the insight that generation is governed by sparse visual-relevant anchors (mandating strictness) amidst abundant visualirrelevant fillers (permitting loose verification), LVSPEC employs a lightweight visual-relevant token identification scheme to accurately pinpoint the former. To further maximize acceptance, we augment this with a position-shift tolerant mechanism that effectively salvages positionally mismatched but semantically equivalent tokens. Experiments demonstrate that LVSPEC achieves high fidelity and speed: it preserves >99.8% of target performance while accelerating Qwen2.5-VL-32B by 2.70× and LLaVA-OneVision-72B by 2.94×. Notably, it boosts the mean accepted length and speedup ratio by 136% and 35% compared to SOTA training-free SD methods for Video-LLMs."
keywords:
  - "see"
  - "forest"
  - "trees"
  - "loosely"
  - "speculative"
  - "decoding"
  - "visual"
  - "semantic"
doi: "10.48550/arxiv.2604.05650"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/corr/abs-2604-05650"
  - name: "arXiv"
    url: "https://arxiv.org/abs/2604.05650v2"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
