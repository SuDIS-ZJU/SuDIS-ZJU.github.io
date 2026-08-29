---
title: "E2USD: Efficient-yet-effective unsupervised state detection for multivariate time series"
authors:
  - "Zhichen Lai"
  - "Huan Li"
  - "Dalin Zhang"
  - "Yan Zhao"
  - "Weizhu Qian"
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
publication: "The ACM Web Conference 2024 (WWW) ORAL"
venue: "The ACM Web Conference 2024 (WWW) ORAL"
publication_kind: "conference"
slug: "paper-c032"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "Cyber-physical system sensors emit multivariate time series (MTS) that monitor physical system processes. Such time series generally capture unknown numbers of states, each with a different duration, that correspond to specific conditions, e.g., “walking” or “running” in human-activity monitoring. Unsupervised identification of such states facilitates storage and processing in subsequent data analyses, as well as enhances result interpretability. Existing state-detection proposals face three challenges. First, they introduce substantial computational overhead, rendering them impractical in resourceconstrained or streaming settings. Second, although state-of-the-art (SOTA) proposals employ contrastive learning for representation, insufficient attention to false negatives hampers model convergence and accuracy. Third, SOTA proposals predominantly only emphasize offline non-streaming deployment, we highlight an urgent need to optimize online streaming scenarios. We propose E2Usd that enables efficient-yet-accurate unsupervised MTS state detection. E2Usd exploits a Fast Fourier Transform-based Time Series Compressor (fftCompress) and a Decomposed Dual-view Embedding Module (ddEM) that together encode input MTSs at low computational overhead. Additionally, we propose a False Negative Cancellation Contrastive Learning method (fnccLearning) to counteract the effects of false negatives and to achieve more cluster-friendly embedding spaces. To reduce computational overhead further in streaming settings, we introduce Adaptive Threshold Detection (adaTD). Comprehensive experiments with six baselines and six datasets offer evidence that E2Usd is capable of SOTA accuracy at significantly reduced computational overhead. Our code is available at https://github.com/AI4CTS/E2Usd."
keywords:
  - "e2usd"
  - "efficient"
  - "yet"
  - "effective"
  - "unsupervised"
  - "state"
  - "detection"
  - "multivariate"
  - "computer science"
  - "interpretability"
doi: "10.1145/3589334.3645593"
aliases:
  - "/en/publication/dblp-confwww-0001-l-00-qj-24/"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/www/0001L00QJ24"
  - name: "arXiv"
    url: "https://arxiv.org/abs/2402.14041"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
