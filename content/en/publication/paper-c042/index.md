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
abstract: "each city constitutes an independent domain with its unique Points of Interest (POIs) and user interaction patterns, where Out-of-Town (OOT) recommendation aims to provide per- sonalized suggestions for users in unfamiliar cities. However, a user’s resident city is considered the source domain, and OOT recommendation faces two fundamental challenges: the the destination city they are visiting is the target domain. difficulty of reasoning across modalities, as preference sig- Existing OOT research (Yin et al. 2016; Ding et al. 2020; nals in disparate formats such as images and text are hard to Li and Gong 2020) often addresses issues like data sparsity compare; and the preference deviation problem, since a user’s and interest drift by developing sophisticated models. How- resident and tourist preferences often diverge, rendering sim- ever, these approaches often overlook two more fundamental ple preference transfer ineffective. To address these chal- challenges in the OOT scenario, limiting their effectiveness lenges, we propose Distinguishing Resident and Tourist Pref- in real-world applications. erences via Multi-Modal LLM Alignment for Out-of-Town The first core challenge is the inherent difficulty of rea- Cross-Domain Recommendation (DiMA), a framework for re-ranking Points of Interest (POIs). To tackle the multimodal soning across modalities (Zhou, Pang, and Li 2024). The challenge, DiMA first leverages Multimodal Large Language appeal of a POI is determined by a combination of its multi- Models and Large Language Models (LLMs) to transform faceted characteristics, which are scattered across different heterogeneous POI data into unified semantic tags, enabling data modalities like images (reflecting facts) and reviews both cross-modal reasoning and efficient downstream pro- (containing sentiments). To determine if a user would like cessing. To address preference deviation, a “teacher” LLM a new venue, the model might need to connect a “vintage at- executes a custom Chain-of-Thought (CoT) process to disen- mosphere” feature from an image the user previously liked tangle resident and tourist preferences from multi-city histo- with a “nostalgic style” mentioned in the new venue’s re- ries for re-ranking. Finally, a lightweight student model learns views. However, since this information exists in entirely dif- this CoT reasoning via Supervised Fine-Tuning and is then ferent formats, it cannot be directly compared or reasoned refined with Direct Preference Optimization to align with true user choices, with the potential to surpass the teacher. with, posing a key bottleneck for achieving precise prefer- Extensive experiments on a real-world dataset demonstrate ence matching. Recently, Large Language Models (LLMs) that DiMA significantly enhances the performance of base- (Liu et al. 2025b,a) have shown promise in solving this prob- line models in the OOT recommendation re-ranking task. lem, but how to guide them for structured reasoning and ef- ficient deployment introduces new questions."
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
