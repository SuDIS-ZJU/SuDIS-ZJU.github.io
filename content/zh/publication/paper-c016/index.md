---
title: "GHive: A demonstration of GPU-accelerated query processing in Apache Hive"
authors:
  - "Haotian Liu"
  - "Bo Tang"
  - "[et al."
  - "including Huan Li]"
date: "2022-01-01"
publishDate: "2022-01-01"
publication_types:
  - "paper-conference"
publication: "2022 ACM SIGMOD/PODS International Conference on Management of Data (SIGMOD)"
slug: "paper-c016"
abstract: "Hive enjoys rapid technical development from the community, and As a distributed, fault-tolerant data warehouse system for large- there are already more than 290 contributors that improve Hive on scale data analytics, Apache Hive has been used for various applica- more than 25,600 issues. For example, Yin et al. introduce optimized tions in many organizations (e.g., Facebook, Amazon and Huawei). columnar file format, physical optimizations, and vectorized query Meanwhile, it is a common practice to exploit the large degrees of execution [5]. Hortonworks Inc. enhances Hive in four different as- parallelism of GPU to improve the performance of online analyt- pects, i.e., SQL and ACID support, optimization techniques, runtime ical processing (OLAP) in database systems. This demo presents latency, and federation capabilities [3]. Up to now, Hive can run on GHive, which enables Apache Hive to accelerate OLAP queries by various execution engines (e.g., Hadoop MapReduce, Apache Tez jointly utilizing CPU and GPU in intelligent and efficient ways. and Spark) by converting an analytical query to a set of executable The takeaways for SIGMOD attendees include: (1) the superior jobs and using Hadoop’s resource negotiator YARN for scheduling. performance of GHive compared with vanilla Hive that only uses In the database community, many systems have been proposed to CPU; (2) intuitive visualizations of execution statistics for Hive and improve the performance of Online Analytical Processing (OLAP) GHive to understand where the acceleration of GHive comes from; with GPUs. In this paper, we present the GHive system, which (3) detailed profiling of the time taken by each operator on CPU improves performance of Hive via CPU-GPU heterogeneous com- and GPU to show the advantages of GPU execution. puting. Different from existing systems that process OLAP queries on GPU [2, 4, 8], GHive supports distributed query processing on CCS CONCEPTS multiple machines with a tailored execution engine. The execution engine comes with optimized implementations of SQL operators • Information systems → Database query processing. and judiciously decides to use GPU or CPU to execute each job"
keywords:
  - "ghive"
  - "demonstration"
  - "gpu"
  - "accelerated"
  - "query"
  - "processing"
  - "apache"
  - "hive"
  - "computer science"
  - "online analytical processing"
doi: "10.1145/3514221.3520166"
aliases:
  - "/zh/publication/dblp-confsigmod-liu-tzdzsyzmzywj-22/"
links:
  - name: "DOI"
    url: "https://doi.org/10.1145/3514221.3520166"
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/sigmod/LiuTZDZSYZMZYWJ22"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
