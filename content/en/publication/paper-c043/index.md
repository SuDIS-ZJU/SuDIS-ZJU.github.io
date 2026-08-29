---
title: "Hierarchical intent-guided optimization with pluggable LLM-Driven semantics for session-based recommendation"
authors:
  - "Jinpeng Chen"
  - "Jianxiang He"
  - "Huan Li"
  - "Senzhang Wang"
  - "Yuan Cao"
  - "Kaimin Wei"
  - "Zhenye Yang"
  - "Ye Ji"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "The 48th International ACM SIGIR Conference on Research and Development in Information Retrieval (SIGIR)"
venue: "The 48th International ACM SIGIR Conference on Research and Development in Information Retrieval (SIGIR)"
publication_kind: "conference"
slug: "paper-c043"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "Session-based Recommendation (SBR) aims to predict the next item a user will likely engage with, using their interaction sequence within an anonymous session. Existing SBR models often focus only on single-session information, ignoring inter-session relationships and valuable cross-session insights. Some methods try to include inter-session data but struggle with noise and irrelevant information, reducing performance. Additionally, most models rely on item ID co-occurrence and overlook rich semantic details, limiting their ability to capture fine-grained item features. To address these challenges, we propose a novel hierarchical intent-guided optimization approach with pluggable LLM-driven semantic learning for session-based recommendations, called HIPHOP. First, we introduce a pluggable embedding module based on large language models (LLMs) to generate high-quality semantic representations, enhancing item embeddings. Second, HIPHOP utilizes graph neural networks (GNNs) to model item transition relationships and incorporates a dynamic multi-intent capturing module to address users' diverse interests within a session. Additionally, we design a hierarchical inter-session similarity learning module, guided by user intent, to capture global and local session relationships, effectively exploring users' long-term and short-term interests. To mitigate noise, an intent-guided denoising strategy is applied during inter-session learning. Finally, we enhance the model's discriminative capability by using contrastive learning to optimize session representations. Experiments on multiple datasets show that HIPHOP significantly outperforms existing methods, demonstrating its effectiveness in improving recommendation quality. Our code is available: https://github.com/hjx159/HIPHOP."
keywords:
  - "hierarchical"
  - "intent"
  - "guided"
  - "optimization"
  - "pluggable"
  - "llm"
  - "driven"
  - "semantics"
  - "session (web analytics)"
  - "computer science"
doi: "10.1145/3726302.3729994"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/sigir/ChenH0WCWYJ25"
  - name: "arXiv"
    url: "https://arxiv.org/abs/2507.04623"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
