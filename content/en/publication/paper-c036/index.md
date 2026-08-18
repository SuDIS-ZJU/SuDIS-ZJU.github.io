---
title: "ReCTSi: Resource-efficient correlated time series imputation via decoupled pattern learning and completeness-aware attentions"
authors:
  - "Zhichen Lai"
  - "Dalin Zhang"
  - "Huan Li"
  - "Dongxiang Zhang"
  - "Hua Lu"
  - "Christian S. Jensen"
date: "2024-01-01"
publishDate: "2024-01-01"
publication_types:
  - "paper-conference"
publication: "The 30th ACM SIGKDD Conference on Knowledge Discovery and Data Mining (KDD)"
slug: "paper-c036"
abstract: "(a) Classical End-to-end Pattern Learning Imputation of Correlated Time Series (CTS) is essential in data pre- Spatial Temporal … Pattern … Pattern … processing for many tasks, particularly when sensor data is often incomplete. Deep learning has enabled sophisticated models that Transient Pattern Adaptation improve CTS imputation by capturing temporal and spatial patterns. … … … However, deep models often incur considerable consumption of CTS Data Spatio- Imputed Shared computational resources and thus cannot be deployed in resource- Input Computational temporal CTS Data Pattern Elements limited settings. This paper presents ReCTSi (Resource-efficient Persistent Pattern Extraction CTS imputation), a method that adopts a new architecture for de- (b) Decoupled Pattern Learning coupled pattern learning in two phases: (1) the Persistent Pattern Ex- Figure 1: Two CTS imputation architectures in inference: (a) traction phase utilizes a multi-view learnable codebook mechanism Classical end-to-end pattern learning, incorporating mul- to identify and archive persistent patterns common across different tiple complex spatial and temporal operators. (b) The pro- time series, enabling rapid pattern retrieval during inference. (2) posed decoupled pattern learning architecture, featuring the the Transient Pattern Adaptation phase introduces completeness- sharing of persistent patterns and lightweight adaptation of aware attention modules that allocate attention to the complete and transient patterns to improve resource-efficiency. hence more reliable data segments. Extensive experimental results show that ReCTSi achieves state-of-the-art imputation accuracy while consuming much fewer computational resources than the"
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
  - name: "DOI"
    url: "https://doi.org/10.1145/3637528.3671816"
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/kdd/000100Z0J24"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
