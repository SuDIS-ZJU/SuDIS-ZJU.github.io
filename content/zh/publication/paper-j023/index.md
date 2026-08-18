---
title: "AdaCTSi: Adaptive Correlated Time Series Imputation for Changing Environments"
authors:
  - "Zhichen Lai"
  - "Huan Li"
  - "Dalin Zhang"
  - "Dong Gong"
  - "Lina Yao"
  - "and Christian S. Jensen"
author_links:
  - name: "Zhichen Lai"
    url: "/authors/zhichen-lai/home/zh/"
date: "2026-01-01"
publishDate: "2026-01-01"
publication_types:
  - "paper-journal"
publication: "IEEE Transactions on Knowledge and Data Engineering (TKDE)"
slug: "paper-j023"
abstract: "Imputation is a well-established data cleaning task within the database community, with deep learning leading the research frontier. In Internet of Things (IoT) applications, vast amounts of Correlated Time Series (CTS) data are generated, often encountering quality issues that necessitate imputation. However, current research predominantly emphasizes accuracy, often neglecting the adaptability required for ever-changing IoT environments. Existing methods struggle with sensor failures because CTS imputation relies on correlations between sensors, cannot selectively impute specific sensors, and use static architectures that fail to adapt to changing resource availability. To tackle these limitations, we propose ADACTSI, an adaptive CTS imputer for changing environments. The architecture integrates a One-shot Temporal Convolutional Network with a Learned Time-Sensor Index Table to extract and decouple complex spatio-temporal features into sensor-wise embeddings, enabling adaptation to inputs from sensor subsets. Sparse Spatial Attention and Correlation-Weighted Sensor Selection identify the most informative sensors and extract spatial correlations. Experiments across twelve baseline methods, three adaptability scenarios, and five benchmark datasets show that ADACTSI reduces MAE by 33.1% on average over the strongest baseline on each dataset, while supporting sensor-subset and resource-adaptive inference with a single trained model. Its modest memory footprint also allows it to run on commodity computing devices, including MCUs."
keywords:
  - "impute on-demand"
  - "adaptive"
  - "correlated time series"
  - "time series imputation"
  - "changing environments"
  - "sensor failure"
  - "resource-adaptive inference"
doi: "10.1109/TKDE.2026.3717792"
links:
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
