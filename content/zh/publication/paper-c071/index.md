---
title: "Bridging Classification and Reconstruction: Cooperative Time Series Anomaly Detection"
authors:
  - "Qideng Tang"
  - "Chaofan Dai"
  - "Wubin Ma"
  - "Yahui Wu"
  - "Haohao Zhou"
  - "Tao Zhang"
  - "Huan Li"
  - "Dalin Zhang"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/zh/"
date: "2026-01-01"
publishDate: "2026-01-01"
publication_types:
  - "paper-conference"
publication: "The 32nd ACM SIGKDD Conference on Knowledge Discovery and Data Mining (KDD)"
venue: "The 32nd ACM SIGKDD Conference on Knowledge Discovery and Data Mining (KDD)"
publication_kind: "conference"
slug: "paper-c071"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "Time series anomaly detection (TSAD) has long been a hot research topic in data mining due to its various applications. Recent studies challenge the effectiveness of popular deep learning methods for TSAD, suggesting their failure in detecting subtle and prolonged anomalies. Outlier Exposure (OE) and Masked Autoencoder (MAE) emerge as two promising paradigms (classification and reconstruction) for solving the above problems. However, OE-based methods are constrained by poor generalization, while MAE-based methods are limited by masking misalignment issues. To address these limitations, this paper proposes a novel framework, CoAD, which unifies the two paradigms to leverage their complementary strengths while mitigating their respective weaknesses. In this framework, the classification module generates probability-informed soft masks for the reconstruction module, which in turn alleviates the generalization problem of the classification module. This cooperative design enables CoAD to effectively detect subtle and complex anomalies that are often overlooked by existing methods. Additionally, the classification module is carefully designed to resolve issues related to improper classification granularity and the neglect of frequency information. Extensive experiments on high-quality benchmark datasets, conducted under rigorous evaluation protocols, demonstrate that CoAD significantly outperforms both state-of-the-art deep learning and traditional data mining methods, highlighting the potential of deep learning in TSAD. Moreover, CoAD is lightweight and substantially faster than existing SOTA methods, demonstrating its practical value for large-scale, real-time applications."
doi: "10.1145/3770855.3818108"
links:
  - name: "arXiv"
    url: "https://arxiv.org/abs/2605.26193"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
