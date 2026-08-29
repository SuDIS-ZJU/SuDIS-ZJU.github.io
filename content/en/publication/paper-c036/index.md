---
title: "ReCTSi: Resource-efficient correlated time series imputation via decoupled pattern learning and completeness-aware attentions"
authors:
  - "Zhichen Lai"
  - "Dalin Zhang"
  - "Huan Li"
  - "Dongxiang Zhang"
  - "Hua Lu"
  - "Christian S. Jensen"
author_links:
  - name: "Zhichen Lai"
    url: "/authors/zhichen-lai/home/"
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2024-01-01"
publishDate: "2024-01-01"
publication_types:
  - "paper-conference"
publication: "The 30th ACM SIGKDD Conference on Knowledge Discovery and Data Mining (KDD)"
venue: "The 30th ACM SIGKDD Conference on Knowledge Discovery and Data Mining (KDD)"
publication_kind: "conference"
slug: "paper-c036"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "Imputation of Correlated Time Series (CTS) is essential in data preprocessing for many tasks, particularly when sensor data is often incomplete. Deep learning has enabled sophisticated models that improve CTS imputation by capturing temporal and spatial patterns. However, deep models often incur considerable consumption of computational resources and thus cannot be deployed in resourcelimited settings. This paper presents ReCTSi (Resource-efficient CTS imputation), a method that adopts a new architecture for decoupled pattern learning in two phases: (1) the Persistent Pattern Extraction phase utilizes a multi-view learnable codebook mechanism to identify and archive persistent patterns common across different time series, enabling rapid pattern retrieval during inference. (2) the Transient Pattern Adaptation phase introduces completenessaware attention modules that allocate attention to the complete and hence more reliable data segments. Extensive experimental results show that ReCTSi achieves state-of-the-art imputation accuracy while consuming much fewer computational resources than the leading existing model, consuming only 0.004% of the FLOPs for inference compared to its closest competitor. The blend of high accuracy and very low resource consumption makes ReCTSi the currently best method for resource-limited scenarios. The related code is available at https://github.com/ryanlaics/RECTSI."
keywords:
  - "rectsi"
  - "resource"
  - "efficient"
  - "correlated"
  - "time"
  - "series"
  - "imputation"
  - "decoupled"
doi: "10.1145/3637528.3671816"
aliases:
  - "/en/publication/dblp-confkdd-000100-z-0-j-24/"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/kdd/000100Z0J24"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
