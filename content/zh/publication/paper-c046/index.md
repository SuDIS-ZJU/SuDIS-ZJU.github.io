---
title: "MovSemCL: Movement-semantics contrastive learning for trajectory similarity"
authors:
  - "Zhichen Lai"
  - "Hua Lu"
  - "李环"
  - "Jialiang Li"
  - "Christian S. Jensen"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "The 40th AAAI Conference on Artificial Intelligence (AAAI) ORAL"
slug: "paper-c046"
abstract: "Trajectory similarity computation is fundamental functional- ity that is used for, e.g., clustering, prediction, and anomaly detection. However, existing learning-based methods ex- hibit three key limitations: (1) insufficient modeling of tra- jectory semantics and hierarchy, lacking both movement dynamics extraction and multi-scale structural representa- tion; (2) high computational costs due to point-wise en- coding; and (3) use of physically implausible augmenta- tions that distort trajectory semantics. To address these is- sues, we propose MovSemCL, a movement-semantics con- trastive learning framework for trajectory similarity com- putation. MovSemCL first transforms raw GPS trajectories into movement-semantics features and then segments them into patches. Next, MovSemCL employs intra- and inter- patch attentions to encode local as well as global trajec- tory patterns, enabling efficient hierarchical representation and reducing computational costs. Moreover, MovSemCL in- cludes a curvature-guided augmentation strategy that pre- serves informative segments (e.g., turns and intersections) Figure 1: Pipeline of MovSemCL. The framework addresses and masks redundant ones, generating physically plausible three limitations: Movement-Semantics Encoding extracts augmented views. Experiments on real-world datasets show movement dynamics (L1), Hierarchical Semantics Encod- that MovSemCL is capable of outperforming state-of-the-art ing captures multi-scale patterns with reduced complexity methods, achieving mean ranks close to the ideal value of 1 (L1, L2), and Semantics-Aware Contrastive Learning uses at similarity search tasks and improvements by up to 20.3% at heuristic approximation, while reducing inference latency curvature-guided augmentation (L3). by up to 43.4%. Code - https://github.com/ryanlaics/MovSemCL and Ratanamahatana 2005; Vlachos, Kollios, and Gunopu- los 2002) are computationally expensive and ignore under"
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
  - name: "DOI"
    url: "https://doi.org/10.1609/aaai.v40i17.38526"
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/aaai/LaiLLLJ26"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
