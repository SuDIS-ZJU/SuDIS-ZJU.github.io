---
title: "Same Last-Item Confusion Unveiled: A Unified Mitigation Framework for Graph Learning in Session-Based Recommendation"
authors:
  - "Jinpeng Chen"
  - "Jianxiang He"
  - "Yuan Cao"
  - "Huan Li"
  - "Zhenye Yang"
  - "Kaimin Wei"
  - "Xiongnan Jin"
  - "Senzhang Wang"
  - "Weiping Tu"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2026-01-01"
publishDate: "2026-01-01"
publication_types:
  - "paper-conference"
publication: "The ACM Web Conference 2026 (WWW)"
venue: "The ACM Web Conference 2026 (WWW)"
publication_kind: "conference"
slug: "paper-c067"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "Session-based recommendation (SBR), which focuses on next-item prediction for anonymous users based on short-term interaction sequences, has garnered increasing attention from researchers. While graph neural networks (GNNs) have become predominant in modeling complex item transition patterns, our empirical study reveals two critical limitations in existing GNN-based SBR methods. On the one hand, they struggle to differentiate between sessions sharing the same last item, resulting in indistinguishable session representations. On the other hand, the inherent popularity bias in session data leads to the over-recommendation of popular items. Inspired by contrastive learning techniques, this paper presents a unified mitigation framework for Same lAst-item confusion in Graph lEarning (SAGE) for SBR. In SAGE, we first obtain normalized session embeddings on constructed session graphs. We then build positive and negative samples of sessions through dual forward propagations and a novel negative sample selection strategy, followed by calculating contrastive loss. Finally, the enhanced session embeddings are utilized for prediction. Extensive experiments on two real-world datasets demonstrate that integrating SAGE with various state-of-the-art GNN-based SBR methods significantly improves their original performances."
keywords:
  - "same"
  - "last"
  - "item"
  - "confusion"
  - "unveiled"
  - "unified"
  - "mitigation"
  - "framework"
  - "graph"
  - "knowledge graph"
doi: "10.1145/3774904.3792356"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/www/ChenHCLYWJWT26"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
