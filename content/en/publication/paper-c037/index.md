---
title: "Revisiting CNNs for trajectory similarity learning"
authors:
  - "Zhihao Chang"
  - "Linzhu Yu"
  - "Huan Li"
  - "Sai Wu"
  - "Gang Chen"
  - "Dongxiang Zhang"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2024-01-01"
publishDate: "2024-01-01"
publication_types:
  - "paper-conference"
publication: "The 50th International Conference on Very Large Data Bases (VLDB)"
venue: "The 50th International Conference on Very Large Data Bases (VLDB)"
publication_kind: "conference"
slug: "paper-c037"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "Similarity search is a fundamental but expensive operator in querying trajectory data, due to its quadratic complexity of distance computation. To mitigate the computational burden for long trajectories, neural networks have been widely employed for similarity learning and each trajectory is encoded as a high-dimensional vector for similarity search with linear complexity. Given the sequential nature of trajectory data, previous efforts have been primarily devoted to the utilization of RNNs or Transformers. In this paper, we argue that the common practice of treating trajectory as sequential data results in excessive attention to capturing long-term global dependency between two sequences. Instead, our investigation reveals the pivotal role of local similarity, prompting a revisit of simple CNNs for trajectory similarity learning. We introduce ConvTraj, incorporating both 1D and 2D convolutions to capture sequential and geo-distribution features of trajectories, respectively. In addition, we conduct a series of theoretical analyses to justify the effectiveness of ConvTraj. Experimental results on four real-world large-scale datasets demonstrate that ConvTraj achieves state-of-the-art accuracy in trajectory similarity search. Owing to the simple network structure of ConvTraj, the training and inference speed on the Porto dataset with 1.6 million trajectories are increased by at least 240x and 2.16x, respectively. The source code and dataset can be found at https://github.com/Proudc/ConvTraj."
keywords:
  - "revisiting"
  - "cnns"
  - "trajectory"
  - "similarity"
  - "learning"
  - "similarity (geometry)"
  - "artificial intelligence"
  - "computer science"
  - "physics"
doi: "10.14778/3717755.3717762"
aliases:
  - "/en/publication/dblp-journalscorrabs-2405-19761/"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/pvldb/ChangYLWCZ24"
  - name: "arXiv"
    url: "https://arxiv.org/abs/2405.19761"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
