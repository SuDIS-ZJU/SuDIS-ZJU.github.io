---
title: "Double: Breaking the Acceleration Limit via Double Retrieval Speculative Parallelism"
authors:
  - "Yuhao Shen"
  - "Tianyu Liu"
  - "Junyi Shen"
  - "Jinyang Wu"
  - "Quan Kong"
  - "Huan Li"
  - "Cong Wang"
date: "2026-01-01"
publishDate: "2026-01-01"
publication_types:
  - "paper-conference"
publication: "The 64th Annual Meeting of the Association for Computational Linguistics (ACL)"
slug: "paper-c059"
abstract: "Parallel Speculative Decoding (PSD) accelerates traditional Speculative Decoding (SD) by overlapping draft generation with verification. However, it remains hampered by two fundamental challenges: (1) a theoretical speedup ceiling dictated by the speed ratio between the draft and target models, and (2) high computational waste and pipeline stall due to mid-sequence token rejections of early errors. To address these limitations, we introduce \\textsc{Double} (Double Retrieval Speculative Parallelism). By bridging the gap between SD and PSD, our framework resolves the Retrieval \\emph{Precision-Efficiency Dilemma} through a novel synchronous mechanism. Specifically, we enable the draft model to execute iterative retrieval speculations to break the theoretical speedup limits; to alleviate rejections without rollback, the target model performs authoritative retrieval to generate multi-token guidance. \\textsc{Double} is entirely training-free and lossless. Extensive experiments demonstrate state-of-the-art speedup of $\\textbf{5.3}\\times$ on LLaMA3.3-70B and $\\textbf{2.8}\\times$ on Qwen3-32B, significantly outperforming the advanced method EAGLE-3 that requires extensive model training."
keywords:
  - "double"
  - "breaking"
  - "acceleration"
  - "limit"
  - "retrieval"
  - "speculative"
  - "parallelism"
  - "speedup"
  - "bridging (networking)"
  - "decoding methods"
links:
  - name: "arXiv"
    url: "https://arxiv.org/abs/2601.05524"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
