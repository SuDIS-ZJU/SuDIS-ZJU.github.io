---
title: "High-throughput ingestion for video warehouse: Comprehensive configuration and effective exploration"
authors:
  - "Baiyan Zhang"
  - "Zepeng Li"
  - "Dongxiang Zhang"
  - "Huan Li"
  - "Kian-Lee Tan"
  - "Gang Chen"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/zh/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "2025 ACM SIGMOD International Conference on Management of Data (SIGMOD)"
venue: "2025 ACM SIGMOD International Conference on Management of Data (SIGMOD)"
publication_kind: "conference"
slug: "paper-c044"
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "The innovative concept of Video Extract-Transform-Load (V-ETL), recently proposed in Skyscraper, reinterprets large-scale video analytics as a data warehousing problem. In this study, we aim at enabling real-time and high-throughput ingestion of hundreds of video streams and maximizing the overall accuracy, by constructing a proper ingestion plan for each video stream. To achieve the goal, we construct a comprehensive configuration space that takes into account the configurable components in the entire ingestion pipeline, including numeric parameters and categorical options such as visual inference model selection. The new space is 10 7 times larger than existing approaches, rendering them as sub-optimal points in our space. To effectively explore the huge and heterogeneous configuration space, we devise an accuracy-aware search strategy based on graph embedding and reinforcement learning to establish the runtime-quality Pareto frontier. To reduce the configuration exploration cost for all video streams, we cluster video streams with similar contexts and adopt mixed integer programming to maximize the overall ingestion accuracy while ensuring the real-time ingestion requirement. In the experimental evaluation with one NVIDIA GeForce RTX 4090 GPU card, our Hippo can support real-time ingestion with 300 video streams and secures an ingestion accuracy that exceeds its competitors by more than 30%."
keywords:
  - "high"
  - "throughput"
  - "ingestion"
  - "video"
  - "warehouse"
  - "comprehensive"
  - "configuration"
  - "effective"
  - "computer science"
  - "pipeline (software)"
doi: "10.1145/3725407"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/pacmmod/ZhangLZLTC25"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
