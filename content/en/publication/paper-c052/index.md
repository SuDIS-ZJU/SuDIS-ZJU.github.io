---
title: "T^2DR: A two-tier deficiency-resistant framework for incomplete multimodal learning"
authors:
  - "Han Lin"
  - "Xiu Tang"
  - "Huan Li"
  - "Wenxue Cao"
  - "Sai Wu"
  - "Chang Yao"
  - "Lidan Shou"
  - "Gang Chen"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "The 63rd Annual Meeting of the Association for Computational Linguistics (ACL) Findings"
venue: "The 63rd Annual Meeting of the Association for Computational Linguistics (ACL) Findings"
publication_kind: "conference"
slug: "paper-c052"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
abstract: "Multimodal learning is garnering significant attention for its capacity to represent diverse human perceptions (e.g., linguistic, acoustic, and visual signals), achieving more natural and intuitive interactions with technology. However, the frequent occurrence of incomplete data, either within a single modality (intra-modality) or across different modalities (inter-modality), presents substantial challenges in reliable semantic interpretation and model reasoning. Furthermore, there is currently no robust representation learning mechanism capable of managing both intra-modality and inter-modality realdata deficiencies. To address this challenge, we present T2DR, a two-tier deficiency-resistant framework for incomplete multimodal learning, which comprises two main modules: (1) IntraModal Deficiency-Resistant module (IADR): To address fine-grained deficiencies, we introduce Intra-Attn to focus on the available data while avoiding excessive suppression of the missing regions. (2) Inter-Modal DeficiencyResistant module (IEDR): To handle coarsegrained deficiencies, we propose the shared feature prediction (SFP) to leverage cross-modal shared features for preliminary data imputation. Subsequently, we apply Inter-Attn to allocate appropriate attention to each modality based on the results from the capability-aware scorer (CAS). Extensive experiments are performed on two well-known multimodal benchmarks, CMU-MOSI and CMU-MOSEI, across various missing scenarios for sentiment analysis. Experimental results show that T2DR significantly outperforms the SOTA models. Code is available at https://github.com/LH019/T2DR."
keywords:
  - "2dr"
  - "two"
  - "tier"
  - "deficiency"
  - "resistant"
  - "framework"
  - "incomplete"
  - "multimodal"
  - "computer science"
  - "artificial intelligence"
doi: "10.18653/v1/2025.findings-acl.452"
links:
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
