---
title: "ScaleSense：基于学习式资源估计的 Alibaba AnalyticDB 成本智能扩缩容框架"
authors:
  - "吴一帆"
  - "Yuhan Li"
  - "Zhenhua Wang"
  - "Ke Chen"
  - "Lidan Shou"
  - "陈宗豪"
  - "Liang Lin"
  - "李环"
  - "Gang Chen"
date: "2026-01-01"
publishDate: "2026-01-01"
publication_types:
  - "paper-conference"
publication: "第 52 届超大规模数据管理国际会议（VLDB）工业赛道"
slug: "paper-c070"
abstract: "云原生无服务器数据仓库通过存储与计算解耦实现细粒度弹性，但面对高度异构的即席查询，如何确定最优资源配置仍是一个严峻的产业挑战。我们对 Alibaba AnalyticDB 生产工作负载的分析揭示了一种代价高昂的“资源配置陷阱”：由于担心资源耗尽造成灾难性影响，用户倾向于盲目过度配置资源，既浪费大量预算，又无法缓解 I/O 饱和等非 CPU 瓶颈。为打破这一困境，本文提出 ScaleSense，一种主动式查询级资源扩缩容框架。该框架设计了多维查询编码器，联合建模查询计划拓扑和硬件规格；更为关键的是，基于分位数的资源预测器能够估计多维物理资源占用，为最优扩缩容提供可靠的安全保障。随后，自动扩缩容控制器沿性能—成本帕累托前沿进行决策，在无需重新训练模型的情况下，根据具体业务优先级动态调整资源配置。在超过 136 万条生产查询上的评测表明，ScaleSense 取得了最先进的预测精度，并具有良好的预测区间覆盖率。相较最佳基线，该方法在最优资源配置选择上的相对效果提升达到 76.7%，同时保持较低的推理开销，验证了其在生产部署中的实用性。在性能优化策略下，ScaleSense 能够满足用户定义的性能要求，并将货币成本最高降低 5.22 倍。"
keywords:
  - "云原生无服务器数据仓库"
  - "查询级资源扩缩容"
  - "资源估计"
  - "自动扩缩容"
  - "成本优化"
doi: "10.14778/3827998.3828016"
links:
  - name: "arXiv"
    url: "https://arxiv.org/abs/2608.07945"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
