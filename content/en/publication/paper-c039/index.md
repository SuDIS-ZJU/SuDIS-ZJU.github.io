---
title: "Beyond fixed variables: Expanding-variate time series forecasting via flat scheme and spatio-temporal focal learning"
authors:
  - "Minbo Ma"
  - "Kai Tang"
  - "Huan Li"
  - "Fei Teng"
  - "Dalin Zhang"
  - "Tianrui Li"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "The 31st ACM SIGKDD Conference on Knowledge Discovery and Data Mining (KDD)"
venue: "The 31st ACM SIGKDD Conference on Knowledge Discovery and Data Mining (KDD)"
publication_kind: "conference"
slug: "paper-c039"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "Multivariate Time Series Forecasting (MTSF) has long been a key research focus. Traditionally, these studies assume a fixed number of variables, but in real-world applications, Cyber-Physical Systems often expand as new sensors are deployed, increasing variables in MTSF. In light of this, we introduce a novel task, Expanding-variate Time Series Forecasting (EVTSF). This task presents unique challenges, specifically (1) handling inconsistent data shapes caused by adding new variables, and (2) addressing imbalanced spatio-temporal learning, where expanding variables have limited observed data due to the necessity for timely operation. To address these challenges, we propose STEV, a flexible spatio-temporal forecasting framework. STEV includes a new Flat Scheme to tackle the inconsistent data shape issue, which extends the graph-based spatio-temporal modeling architecture into 1D space by flattening the 2D samples along the variable dimension, making the model variable-scale-agnostic while still preserving dynamic spatial correlations through a holistic graph. We introduce a novel Spatio-temporal Focal Learning strategy that incorporates a negative filter to resolve potential conflicts between contrastive learning and graph representation, and a focal contrastive loss as its core to guide the framework to focus on optimizing the expanding variables. We benchmark EVTSF performance using three real-world datasets and compare it against three potential solutions employing SOTA MTSF models tailored for EVSTF. Experimental results show that STEV significantly outperforms its competitors, particularly on expanding variables. Notably, STEV, with only 5% of observations from the expanding period, is on par with SOTA MTSF models trained with complete observations. Further exploration of various expanding strategies underscores the generalizability of STEV in real-world applications."
keywords:
  - "beyond"
  - "fixed"
  - "variables"
  - "expanding"
  - "variate"
  - "time"
  - "series"
  - "forecasting"
  - "random variate"
  - "series (stratigraphy)"
doi: "10.1145/3711896.3736854"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/kdd/MaT000025"
  - name: "arXiv"
    url: "https://arxiv.org/abs/2502.15296"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
