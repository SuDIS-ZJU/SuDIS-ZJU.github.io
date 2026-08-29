---
title: "STEP: Stepwise curriculum learning for context-knowledge fusion in conversational recommendation"
authors:
  - "Zhenye Yang"
  - "Jinpeng Chen"
  - "Huan Li"
  - "et al"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "The 34th ACM International Conference on Information & Knowledge Management (CIKM)"
venue: "The 34th ACM International Conference on Information & Knowledge Management (CIKM)"
publication_kind: "conference"
slug: "paper-c051"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-B"
  - "CORE-A"
abstract: "Conversational recommender systems (CRSs) aim to proactively capture user preferences through natural language dialogue and recommend high-quality items. To achieve this, CRS gathers user preferences via a dialog module and builds user profiles through a recommendation module to generate appropriate recommendations. However, existing CRS faces challenges in capturing the deep semantics of user preferences and dialogue context. In particular, the efficient integration of external knowledge graph (KG) information into dialogue generation and recommendation remains a pressing issue. Traditional approaches typically combine KG information directly with dialogue content, which often struggles with complex semantic relationships, resulting in recommendations that may not align with user expectations. To address these challenges, we introduce STEP, a conversational recommender centered on pre-trained language models that combines curriculum-guided context-knowledge fusion with lightweight task-specific prompt tuning. At its heart, an F-Former progressively aligns the dialogue context with knowledge-graph entities through a three-stage curriculum, thus resolving fine-grained semantic mismatches. The fused representation is then injected into the frozen language model via two minimal yet adaptive prefix prompts: a conversation prefix that steers response generation toward user intent and a recommendation prefix that biases item ranking toward knowledge-consistent candidates. This dual-prompt scheme allows the model to share cross-task semantics while respecting the distinct objectives of dialogue and recommendation. Experimental results show that STEP outperforms mainstream methods in the precision of recommendation and dialogue quality in two public datasets."
keywords:
  - "step"
  - "stepwise"
  - "curriculum"
  - "learning"
  - "context"
  - "knowledge"
  - "fusion"
  - "conversational"
  - "dialog box"
  - "semantics (computer science)"
doi: "10.1145/3746252.3761186"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/cikm/Yang0LJLZ0WW25"
  - name: "arXiv"
    url: "https://arxiv.org/abs/2508.10669"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
