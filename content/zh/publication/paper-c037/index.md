---
title: "Revisiting CNNs for trajectory similarity learning"
authors:
  - "Zhihao Chang"
  - "Linzhu Yu"
  - "李环"
  - "Sai Wu"
  - "Gang Chen"
  - "Dongxiang Zhang"
date: "2024-01-01"
publishDate: "2024-01-01"
publication_types:
  - "paper-conference"
publication: "The 50th International Conference on Very Large Data Bases (VLDB)"
slug: "paper-c037"
abstract: "I need to buy some food from the store. [cs.AI] 5 Nov 2024 Similarity search is a fundamental but expensive operator in query- I need to go to the store to buy some food. ing trajectory data, due to its quadratic complexity of distance com- (a) Text semantic similarity (b) Trajectory similarity based DFD putation. To mitigate the computational burden for long trajectories, neural networks have been widely employed for similarity learning Figure 1: Texts feature intercrossed matching pairs, whereas and each trajectory is encoded as a high-dimensional vector for sim- trajectories do not. ilarity search with linear complexity. Given the sequential nature of trajectory data, previous efforts have been primarily devoted to the utilization of RNNs or Transformers. Given the sequential nature of trajectory data, existing methods In this paper, we argue that the common practice of treating tra- for trajectory similarity learning can be categorized into RNN- jectory as sequential data results in excessive attention to capturing based or Transformer-based. RNN-based methods, including Neu- long-term global dependency between two sequences. Instead, our Traj [31], Traj2SimVec [36], and T3S [30], employ RNN or its vari- investigation reveals the pivotal role of local similarity, prompting ants (e.g, GRU [13], LSTM [18]) as the core encoder, which can be a revisit of simple CNNs for trajectory similarity learning. We in- augmented with additional components such as spatial attention troduce ConvTraj, incorporating both 1D and 2D convolutions to memory in NeuTraj and point or structure matching mechanisms capture sequential and geo-distribution features of trajectories, re- in Traj2SimVec and T3S to enhance performance. Due to the suc- spectively. In addition, we conduct a series of theoretical analyses to cess of Transformer in NLP, TrajGAT [32] and TrajCL [7] adopt justify the effectiveness of ConvTraj. Experimental results on four Transformer to learn trajectory embedding, which can effectively real-world large-scale datasets demonstrate that ConvTraj achieves capture the long-term dependency of sequences. state-of-the-art accuracy in trajectory similarity search. Owing to However, we argue that these common practices pay excessive the simple network structure of ConvTraj, the training and infer- attention to capturing long-term global dependency between two ence speed on the Porto dataset with 1.6 million trajectories are trajectories while ignoring point-wise similarity, which may poten- increased by at least 240x and 2.16x, respectively. The source code tially yield adverse effects. Instead, we should pay more attention and dataset can be found at https:// github.com/ Proudc/ ConvTraj. to point-wise similarity in the local context. In support of this argu- ment, we conducted an experiment on Porto1 dataset to evaluate the effect of applying Transformer for trajectory encoding with"
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
  - "/zh/publication/dblp-journalscorrabs-2405-19761/"
links:
  - name: "DOI"
    url: "https://doi.org/10.14778/3717755.3717762"
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/pvldb/ChangYLWCZ24"
  - name: "arXiv"
    url: "https://arxiv.org/abs/2405.19761"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
