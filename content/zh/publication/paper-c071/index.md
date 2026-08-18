---
title: "融合分类与重构：协同式时间序列异常检测"
authors:
  - "Qideng Tang"
  - "Chaofan Dai"
  - "Wubin Ma"
  - "Yahui Wu"
  - "Haohao Zhou"
  - "Tao Zhang"
  - "李环"
  - "Dalin Zhang"
date: "2026-01-01"
publishDate: "2026-01-01"
publication_types:
  - "paper-conference"
publication: "第 32 届 ACM 知识发现与数据挖掘大会（KDD）"
slug: "paper-c071"
abstract: "时间序列异常检测（TSAD）因其广泛的应用场景，长期以来一直是数据挖掘领域的研究热点。近期研究对流行的深度学习方法在 TSAD 中的有效性提出了质疑，指出这些方法难以检测细微且持续时间较长的异常。离群暴露（OE）和掩码自编码器（MAE）分别代表分类式和重构式两种有前景的解决范式。然而，基于 OE 的方法受到泛化能力不足的限制，基于 MAE 的方法则受掩码错位问题影响。为解决上述局限，本文提出 CoAD，一种统一两种范式的新型框架，通过发挥二者的互补优势并缓解各自的缺陷，实现更有效的异常检测。在该框架中，分类模块为重构模块生成包含概率信息的软掩码，从而缓解分类模块的泛化问题。这种协同设计能够有效检测容易被现有方法忽略的细微和复杂异常。此外，分类模块经过专门设计，解决了分类粒度不当以及忽视频率信息的问题。在高质量基准数据集上按照严格评测协议开展的大量实验表明，CoAD 显著优于当前最优的深度学习方法和传统数据挖掘方法，展现了深度学习在 TSAD 中的潜力。同时，CoAD 轻量且明显快于现有最优方法，体现出其在大规模实时应用中的实际价值。"
keywords:
  - "时间序列异常检测"
  - "离群暴露"
  - "掩码自编码器"
  - "协同学习"
  - "分类与重构"
doi: "10.1145/3770855.3818108"
links:
  - name: "arXiv"
    url: "https://arxiv.org/abs/2605.26193"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
