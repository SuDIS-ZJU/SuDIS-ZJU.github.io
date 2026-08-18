---
title: "Not all data are good labels: On the self-supervised labeling for time series forecasting"
authors:
  - "Yuxuan Yang"
  - "Dalin Zhang"
  - "Yuxuan Liang"
  - "Hua Lu"
  - "Gang Chen"
  - "Huan Li"
author_links:
  - name: "Yuxuan Yang"
    url: "/authors/yuxuan-yang/home/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "The 39 Annual Conference on Neural Information Processing Systems (NeurIPS)"
slug: "paper-c048"
abstract: "Time Series Forecasting (TSF) is a crucial task in various domains, yet existing TSF models rely heavily on high-quality data and insufficiently exploit all available data. This paper explores a novel self-supervised approach to re-label time series datasets by inherently constructing candidate datasets. During the optimization of a simple reconstruction network, intermediates are used as pseudo labels in a self-supervised paradigm, improving generalization for any predictor. We introduce the Self- Correction with Adaptive Mask (S CAM), which discards overfitted components and selectively replaces them with pseudo labels generated from reconstructions. Additionally, we incorporate Spectral Norm Regularization (SNR) to further sup- press overfitting from a loss landscape perspective. Our experiments on eleven real-world datasets demonstrate that S CAM consistently improves the performance of various backbone models. This work offers a new perspective on constructing datasets and enhancing the generalization of TSF models through self-supervised learning. The code is available at https://github.com/SuDIS-ZJU/SCAM."
keywords:
  - "not"
  - "all"
  - "data"
  - "good"
  - "labels"
  - "self"
  - "supervised"
  - "labeling"
  - "series (stratigraphy)"
  - "computer science"
doi: "10.48550/arxiv.2502.14704"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/corr/abs-2502-14704"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
