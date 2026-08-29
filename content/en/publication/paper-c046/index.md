---
title: "MovSemCL: Movement-semantics contrastive learning for trajectory similarity"
authors:
  - "Zhichen Lai"
  - "Hua Lu"
  - "Huan Li"
  - "Jialiang Li"
  - "Christian S. Jensen"
author_links:
  - name: "Zhichen Lai"
    url: "/authors/zhichen-lai/home/"
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "The 40th AAAI Conference on Artificial Intelligence (AAAI) ORAL"
venue: "The 40th AAAI Conference on Artificial Intelligence (AAAI) ORAL"
publication_kind: "conference"
slug: "paper-c046"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A"
abstract: "Trajectory similarity computation is fundamental functionality that is used for, e.g., clustering, prediction, and anomaly detection. However, existing learning-based methods exhibit three key limitations: (1) insufficient modeling of trajectory semantics and hierarchy, lacking both movement dynamics extraction and multi-scale structural representation; (2) high computational costs due to point-wise encoding; and (3) use of physically implausible augmentations that distort trajectory semantics. To address these issues, we propose MovSemCL, a movement-semantics contrastive learning framework for trajectory similarity computation. MovSemCL first transforms raw GPS trajectories into movement-semantics features and then segments them into patches. Next, MovSemCL employs intra- and interpatch attentions to encode local as well as global trajectory patterns, enabling efficient hierarchical representation and reducing computational costs. Moreover, MovSemCL includes a curvature-guided augmentation strategy that preserves informative segments (e.g., turns and intersections) and masks redundant ones, generating physically plausible augmented views. Experiments on real-world datasets show that MovSemCL is capable of outperforming state-of-the-art methods, achieving mean ranks close to the ideal value of 1 at similarity search tasks and improvements by up to 20.3% at heuristic approximation, while reducing inference latency by up to 43.4%."
keywords:
  - "movsemcl"
  - "movement"
  - "semantics"
  - "contrastive"
  - "learning"
  - "trajectory"
  - "similarity"
doi: "10.1609/aaai.v40i17.38526"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/aaai/LaiLLLJ26"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
