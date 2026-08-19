---
title: "GHive: Accelerating analytical query processing in Apache Hive via CPU-GPU heterogeneous computing"
authors:
  - "Haotian Liu"
  - "Bo Tang"
  - "[et al."
  - "including Huan Li]"
date: "2022-01-01"
publishDate: "2022-01-01"
publication_types:
  - "paper-conference"
publication: "13th Symposium on Cloud Computing (ACM SoCC) -- SIGMOD and SIGOPS co-sponsored"
venue: "13th Symposium on Cloud Computing (ACM SoCC) -- SIGMOD and SIGOPS co-sponsored"
publication_kind: "conference"
slug: "paper-c017"
venue_rankings:
  - "CCF-B"
abstract: "As a popular distributed data warehouse system, Apache Hive has been widely used for big data analytics in many organizations. Meanwhile, exploiting the massive parallelism of GPU to accelerate online analytical processing (OLAP) has been extensively explored in the database community. In this paper, we present GHive, which enhances CPU-based Hive via CPU-GPU heterogeneous computing. GHive is designed for the business intelligence applications and provides the same API as Hive for compatibility. To run SQL queries jointly on both CPU and GPU, GHive comes with three key techniques: (i) a novel data model gTable, which is column-based and enables efficient data movement between CPU memory and GPU memory; (ii) a GPU-based operator library Panda, which provides a complete set of SQL operators with extensively optimized GPU implementations; (iii) a hardware-aware MapReduce job placement scheme, which puts jobs judiciously on either GPU or CPU via a cost-based approach. In the experiments, we observe that GHive outperforms Hive in both query processing speed and operating expense on the Star Schema Benchmark (SSB)."
keywords:
  - "ghive"
  - "accelerating"
  - "analytical"
  - "query"
  - "processing"
  - "apache"
  - "hive"
  - "cpu"
doi: "10.1145/3542929.3563503"
aliases:
  - "/zh/publication/dblp-confcloud-liu-0-zd-0-zszmzywj-22/"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/cloud/Liu0ZD0ZSZMZYWJ22"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
