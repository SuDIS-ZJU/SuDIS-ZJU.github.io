---
title: "面向变化环境的自适应相关时间序列插补"
authors:
  - "Zhichen Lai"
  - "李环"
  - "Dalin Zhang"
  - "Dong Gong"
  - "Lina Yao"
  - "and Christian S. Jensen"
date: "2026-01-01"
publishDate: "2026-01-01"
publication_types:
  - "paper-journal"
publication: "IEEE Knowledge and Data Engineering Transactions（TKDE）"
slug: "paper-j023"
abstract: "插补是数据库领域中成熟的数据清洗任务，深度学习已成为该方向的研究前沿。在物联网（IoT）应用中，大量相关时间序列（CTS）数据持续产生，并且经常存在需要插补的数据质量问题。然而，现有研究主要关注精度，往往忽视物联网环境持续变化所要求的适应能力。现有方法难以应对传感器故障：相关时间序列插补依赖传感器之间的相关性，无法选择性地对指定传感器进行插补，并且采用静态架构，难以适应不断变化的资源可用性。为此，本文提出面向变化环境的自适应 CTS 插补方法 ADACTSI。该方法将一次性时间卷积网络与学习式时间—传感器索引表相结合，从复杂的时空特征中提取并解耦传感器级嵌入，从而适应来自不同传感器子集的输入。稀疏空间注意力和相关性加权的传感器选择机制用于识别信息量最大的传感器并提取空间相关性。在 12 种基线方法、3 类适应性场景和 5 个基准数据集上的实验表明，ADACTSI 在各数据集上相对最强基线平均降低 33.1% 的 MAE，同时支持传感器子集推理和资源自适应推理，并且只需一个训练好的模型。其较小的内存占用还使其能够运行在包括微控制器（MCU）在内的通用计算设备上。"
keywords:
  - "按需插补"
  - "自适应推理"
  - "相关时间序列"
  - "时间序列插补"
  - "变化环境"
  - "传感器故障"
  - "资源自适应推理"
doi: "10.1109/TKDE.2026.3717792"
links:
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
