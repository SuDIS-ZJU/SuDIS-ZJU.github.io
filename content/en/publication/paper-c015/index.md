---
title: "Efficient and error-bounded spatiotemporal quantile monitoring in edge computing environments"
authors:
  - "Huan Li"
  - "Lanjing Yi"
  - "Bo Tang"
  - "Hua Lu"
  - "Christian S. Jensen"
date: "2022-01-01"
publishDate: "2022-01-01"
publication_types:
  - "paper-conference"
publication: "The 48th International Conference on Very Large Data Bases (VLDB)"
slug: "paper-c015"
abstract: "Underlying many types of data analytics, a spatiotemporal quantile monitoring (SQM) query continuously returns the quantiles of a dataset observed in a spatiotemporal range. In this paper, we study SQM in an Internet of Things (IoT) based edge computing environment, where concurrent SQM queries share the same infrastructure asynchronously. To minimize query latency while providing result accuracy guarantees, we design a processing framework that virtualizes edge-resident data sketches for quantile computing. In the framework, a coordinator edge node manages edge sketches and synchronizes edge sketch processing and query executions. The co-ordinator also controls the processed data fractions of edge sketches, which helps to achieve the optimal latency with error-bounded results for each single query. To support concurrent queries, we employ a grid to decompose queries into subqueries and process them efficiently using shared edge sketches. We also devise a relaxation algorithm to converge to optimal latencies for those subqueries whose result errors are still bounded. We evaluate our proposals using two high-speed streaming datasets in a simulated IoT setting with edge nodes. The results show that our proposals achieve efficient, scalable, and error-bounded SQM."
keywords:
  - "efficient"
  - "error"
  - "bounded"
  - "spatiotemporal"
  - "quantile"
  - "monitoring"
  - "edge"
  - "computing"
  - "bounded function"
  - "enhanced data rates for gsm evolution"
doi: "10.14778/3538598.3538600"
aliases:
  - "/en/publication/dblp-journalspvldb-li-ytlj-22/"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/pvldb/LiYTLJ22"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
