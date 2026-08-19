---
title: "Transfer-Aware Data Selection for Domain Adaptation in Text Retrieval"
authors:
  - "Linzhu Yu"
  - "Huan Li"
  - "Ke Chen"
  - "Lidan Shou"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/zh/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "The 2025 Conference on Empirical Methods in Natural Language Processing (EMNLP) Findings"
venue: "The 2025 Conference on Empirical Methods in Natural Language Processing (EMNLP) Findings"
publication_kind: "conference"
slug: "paper-c057"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-B"
  - "CORE-A"
abstract: "Domain adaptation is widely adopted in text retrieval scenarios where large labeled data is unavailable. To improve model adaptability, existing methods try to expand more source datasets. However, we found from experiments that indiscriminately using a large amount of source data from various text tasks does not guarantee improved adaptability, but may negatively impact ranking model performance. To tackle this issue, we propose Trait, a framework that can effectively improve model adaptability by selecting beneficial data without evaluating all source data. Specifically, we first divide multiple source datasets into data chunks of the same size as the minimum selection unit to form the whole selection space. Then we devise an iterative process that includes Bayesian optimization-based selection and transfer-aware chunk evaluation to incrementally select beneficial chunks. To reduce unnecessary evaluation costs, we also design backtracking and pruning actions to adjust the selection subspace. Extensive experimental results show that Trait not only achieves average state-of-the-art for few-shot on nine target datasets by evaluating only 4% of BERRI source data, but is also highly competitive for zero-shot compared with LLM-based rankers."
keywords:
  - "transfer"
  - "aware"
  - "data"
  - "selection"
  - "domain"
  - "adaptation"
  - "text"
  - "retrieval"
  - "computer science"
  - "artificial intelligence"
doi: "10.18653/v1/2025.findings-emnlp.948"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/emnlp/YuLCS25"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
