---
title: "ChronosBI：基于语义缓存与成本规划的 LLM 驱动商业智能流水线增强系统"
authors:
  - "张剑峰"
  - "崔凌睎"
  - "Yongqin Xu"
  - "王童"
  - "Yi Guo"
  - "Zhouzhi Yang"
  - "李环"
  - "Ke Chen"
  - "Lidan Shou"
date: "2026-01-01"
publishDate: "2026-01-01"
publication_types:
  - "paper-conference"
publication: "2026 ACM 数据管理国际会议（SIGMOD）Demo"
slug: "paper-c058"
abstract: "现代商业智能（BI）系统越来越多地依赖大语言模型（LLM），将自然语言（NL）查询转换为可执行的领域特定语言（DSL）程序。然而，现有多阶段长链式 LLM 流水线面临高延迟、令牌开销高和错误传播等问题，限制了其在真实企业环境中的部署。本文介绍 ChronosBI，这是一个端到端、以效率为导向的 BI 系统，展示了 LLM 驱动分析的一种新型执行范式。ChronosBI 集成了两个协同工作的模块：（1）智能缓存引擎，通过基于骨架的匹配和少样本 DSL 生成，加速重复或结构相似的自然语言查询；（2）强化学习成本规划器，在缓存失效时动态优化长链式流水线，通过跳过不必要的步骤降低成本，同时保持准确率。ChronosBI 已部署于小红书，每日服务超过 5,000 个会话，在保持 84.64% 准确率的同时实现了 2 倍加速。访问者可以通过在线演示体验这一自适应、成本感知的生成过程，该系统展示了下一代 LLM 商业智能系统实现规模化部署的一条可行路径。"
keywords:
  - "ChronosBI"
  - "大语言模型"
  - "商业智能"
  - "语义缓存"
  - "成本规划"
  - "自然语言到领域特定语言"
doi: "10.1145/3788853.3801580"
links:
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
