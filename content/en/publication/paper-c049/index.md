---
title: "SafeLoad: Efficient admission control framework for identifying memory-overloading queries in cloud data warehouses"
authors:
  - "Yifan Wu"
  - "Yuhan Li"
  - "Zhenhua Wang"
  - "Zhongle Xie"
  - "Dingyu Yang"
  - "Ke Chen"
  - "Lidan Shou"
  - "Bo Tang"
  - "Liang Lin"
  - "Huan Li"
  - "Gang Chen"
author_links:
  - name: "Yifan Wu"
    url: "/authors/yifan-wu/home/"
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "The 51th International Conference on Very Large Data Bases (VLDB)"
venue: "The 51th International Conference on Very Large Data Bases (VLDB)"
publication_kind: "conference"
slug: "paper-c049"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "Memory overload is a common form of resource exhaustion in cloud data warehouses. When database queries fail due to memory overload, it not only wastes critical resources such as CPU time but also disrupts the execution of core business processes, as memory-overloading (MO) queries are typically part of complex workflows. If such queries are identified in advance and scheduled to memory-rich serverless clusters, it can prevent resource wastage and query execution failure. Therefore, cloud data warehouses desire an admission control framework with high prediction precision, interpretability, efficiency, and adaptability to effectively identify memory-overloading queries. However, existing admission control frameworks primarily focus on scenarios like SLA satisfaction and resource isolation, with limited precision in identifying MO queries. Moreover, there is a lack of publicly available MO-labeled datasets with workloads for training and benchmarking. To tackle these challenges, we propose SafeLoad, the first query admission control framework specifically designed to identify MO queries. Alongside, we release SafeBench, an open-source, industrial-scale benchmark for this task, which includes 150 million real queries. SafeLoad first filters out memory-safe queries using the interpretable discriminative rule. It then applies a hybrid architecture that integrates both a global model and cluster-level models, supplemented by a misprediction correction module to identify MO queries. Additionally, a self-tuning quota management mechanism dynamically adjusts prediction quotas per cluster to improve precision. Experimental results show that SafeLoad achieves state-of-the-art prediction performance with low online and offline time overhead. Specifically, SafeLoad improves precision by up to 66% over the best baseline and reduces wasted CPU time by up to 8.09× compared to scenarios without SafeLoad."
keywords:
  - "safeload"
  - "efficient"
  - "admission"
  - "control"
  - "framework"
  - "identifying"
  - "memory"
  - "overloading"
doi: "10.14778/3785297.3785311"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/corr/abs-2601-01888"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
