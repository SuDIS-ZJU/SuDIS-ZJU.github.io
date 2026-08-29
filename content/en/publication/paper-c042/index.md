---
title: "DiMA: Distinguishing resident and tourist preferences via multi-modal LLM alignment for out-of-town cross-domain recommendation"
authors:
  - "Fan Zhang"
  - "Jinpeng Chen"
  - "Tao Wang"
  - "Huan Li"
  - "Senzhang Wang"
  - "Feifei Kou"
  - "Ji Ye"
  - "Kaimin Wei"
  - "and Zhenye Yang"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "The 40th AAAI Conference on Artificial Intelligence (AAAI) ORAL"
venue: "The 40th AAAI Conference on Artificial Intelligence (AAAI) ORAL"
publication_kind: "conference"
slug: "paper-c042"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A"
abstract: "Out-of-Town (OOT) recommendation aims to provide personalized suggestions for users in unfamiliar cities. However, OOT recommendation faces two fundamental challenges: the difficulty of reasoning across modalities, as preference signals in disparate formats such as images and text are hard to compare; and the preference deviation problem, since a user’s resident and tourist preferences often diverge, rendering simple preference transfer ineffective. To address these challenges, we propose Distinguishing Resident and Tourist Preferences via Multi-Modal LLM Alignment for Out-of-Town Cross-Domain Recommendation (DiMA), a framework for re-ranking Points of Interest (POIs). To tackle the multimodal challenge, DiMA first leverages Multimodal Large Language Models and Large Language Models (LLMs) to transform heterogeneous POI data into unified semantic tags, enabling both cross-modal reasoning and efficient downstream processing. To address preference deviation, a “teacher” LLM executes a custom Chain-of-Thought (CoT) process to disentangle resident and tourist preferences from multi-city histories for re-ranking. Finally, a lightweight student model learns this CoT reasoning via Supervised Fine-Tuning and is then refined with Direct Preference Optimization to align with true user choices, with the potential to surpass the teacher. Extensive experiments on a real-world dataset demonstrate that DiMA significantly enhances the performance of baseline models in the OOT recommendation re-ranking task."
keywords:
  - "dima"
  - "distinguishing"
  - "resident"
  - "tourist"
  - "preferences"
  - "multi"
  - "modal"
  - "llm"
doi: "10.1609/aaai.v40i19.38663"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/aaai/ZhangCWLWKJWY26"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
