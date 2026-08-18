---
title: "ParallelVLM: Lossless Video-LLM Acceleration with Visual Alignment Aware Parallel Speculative Decoding"
authors:
  - "Quan Kong"
  - "Yuhao Shen"
  - "Yicheng Ji"
  - "Huan Li"
  - "Cong Wang"
author_links:
  - name: "Yicheng Ji"
    url: "/authors/yicheng-ji/home/zh/"
date: "2026-01-01"
publishDate: "2026-01-01"
publication_types:
  - "paper-conference"
publication: "The IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)"
slug: "paper-c065"
abstract: "Although current Video-LLMs achieve impressive performance in video understanding tasks, their autoregressive decoding efficiency remains constrained by the massive number of video tokens. Visual token pruning can partially ease this bottleneck, yet existing approaches still suffer from information loss and yield only modest acceleration in decoding. In this paper, we propose ParallelVLM, a training-free draft-then-verify speculative decoding framework that overcomes both mutual waiting and limited speedup-ratio problems between draft and target models in long-video settings. ParallelVLM features two parallelized stages that maximize hardware utilization and incorporate an Unbiased Verifier-Guided Pruning strategy to better align the draft and target models by eliminating the positional bias in attention-guided pruning. Extensive experiments demonstrate that ParallelVLM effectively expands the draft window by 1.6–1.8× with high accepted lengths, and accelerates various video understanding benchmarks by 3.36× on LLaVA-OneVision-72B and 2.42× on Qwen2.5-VL-32B compared with vanilla autoregressive decoding. Codes are available at https://github.com/imKQv/ParallelVLM."
keywords:
  - "parallelvlm"
  - "lossless"
  - "video"
  - "llm"
  - "acceleration"
  - "visual"
  - "alignment"
  - "aware"
  - "decoding methods"
  - "pruning"
links:
  - name: "arXiv"
    url: "https://arxiv.org/abs/2603.19610"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
