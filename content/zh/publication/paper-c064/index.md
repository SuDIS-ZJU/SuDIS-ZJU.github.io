---
title: "Mitigating Noise-Induced Layout Priors for Object Counting in Diffusion Models"
authors:
  - "Xiaoling Gu"
  - "Xuelong Li"
  - "Shengqi Wu"
  - "Yongkang Wong"
  - "Zizhao Wu"
  - "李环"
  - "Zhou Yu"
  - "and Mohan Kankanhalli"
date: "2026-01-01"
publishDate: "2026-01-01"
publication_types:
  - "paper-conference"
publication: "The 43th International Conference on Machine Learning (ICML)"
slug: "paper-c064"
abstract: "Despite remarkable progress in text-to-image diffusion models, accurately generating the specified number of objects remains a persistent challenge. We identify the initial noise as a primary determinant of spatial layout formation, with early-stage cross-attention serving as the key mechanism that mediates the propagation of noise-induced structures throughout the denoising process. We characterize this phenomenon as Noise-Induced Layout Prior. Leveraging this insight, we propose a novel training-free framework for object counting in diffusion models. Our approach consists of two key components: (1) a Count-Aware Noise Adjustment Strategy, which explicitly manipulates the initial latent noise to align layout formation with the target object count, and (2) an Attention-Guided Layout Consistency Strategy, which performs test-time optimization on early-stage cross-attention to further stabilize layout formation during denoising. Extensive experiments on both single-category and multi-category benchmarks demonstrate that our method consistently outperforms strong diffusion baselines and state-of-the-art object count control methods in terms of counting accuracy and image quality. Code Release: https://github.com/lxlong1201/Mitigate_Noise_Prior."
keywords:
  - "mitigating"
  - "noise"
  - "induced"
  - "layout"
  - "priors"
  - "object"
  - "counting"
  - "diffusion"
links:
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
