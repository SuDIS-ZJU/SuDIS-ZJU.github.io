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
abstract: "Query Optimizer Executor Executor Executor Memory overload is a common form of resource exhaustion in SQL Queries cloud data warehouses. When database queries fail due to mem- ory overload, it not only wastes critical resources such as CPU Cloud Data Warehouses without SafeLoad Failure of All Memory-Overloading Queries Safe Queries time but also disrupts the execution of core business processes, as memory-overloading (MO) queries are typically part of complex Significant CPU Time Wastage workflows. If such queries are identified in advance and scheduled join Query Plan Statistics scan scan to memory-rich serverless clusters, it can prevent resource wastage Query Optimizer SafeLoad and query execution failure. Therefore, cloud data warehouses de- SQL Queries Resource Metrics Resource Monitor sire an admission control framework with high prediction precision, interpretability, efficiency, and adaptability to effectively identify Cloud Data Warehouses with SafeLoad Memory-Overloading Queries memory-overloading queries. However, existing admission control Reduction in Memory-Overloading Queries frameworks primarily focus on scenarios like SLA satisfaction and Reduction in Wasted CPU Time Executor Executor Executor resource isolation, with limited precision in identifying MO queries. Serverless Cluster Moreover, there is a lack of publicly available MO-labeled datasets Figure 1: The role of SafeLoad in cloud data warehouses. with workloads for training and benchmarking. To tackle these chal- lenges, we propose SafeLoad, the first query admission control doi:XX.XX/XXX.XX framework specifically designed to identify MO queries. Alongside, PVLDB Artifact Availability: we release SafeBench, an open-source, industrial-scale benchmark The source code, data, and/or other artifacts have been made available at for this task, which includes 150 million real queries. SafeLoad first https://github.com/SafeLoad-project/SafeBench. filters out memory-safe queries using the interpretable discrimina- tive rule. It then applies a hybrid architecture that integrates both"
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
