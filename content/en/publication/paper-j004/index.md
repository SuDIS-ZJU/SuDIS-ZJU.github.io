---
title: "Towards indoor temporal-variation aware shortest path query"
authors:
  - "Tiantian Liu"
  - "Zijin Feng"
  - "Huan Li"
  - "Hua Lu"
  - "Muhammad Aamir Cheema"
  - "Hong Cheng"
  - "Jianliang Xu"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2021-01-01"
publishDate: "2021-01-01"
publication_types:
  - "paper-journal"
publication: "IEEE Transactions on Knowledge and Data Engineering (TKDE)"
venue: "IEEE Transactions on Knowledge and Data Engineering (TKDE)"
publication_kind: "journal"
slug: "paper-j004"
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "The recent years have witnessed the growing popularity of indoor location-based services (LBS) in practice and research. Among others, indoor shortest path query (ISPQ) is of fundamental importance for indoor LBS. However, existing works on ISPQ ignore indoor temporal variations, e.g., the open and close times associated with entities like doors and rooms. In this paper, we define a new type of query called Indoor Temporal-variation aware Shortest Path Query (ITSPQ). It returns the valid shortest path based on the up-to-date indoor topology at the query time. A set of techniques is designed to answer ITSPQ efficiently. We design a graph structure (IT-Graph) that captures indoor temporal variations. To process ITSPQ using IT-Graph, we design two algorithms that check a door’s accessibility synchronously and asynchronously. Furthermore, we propose a novel index structure (IT-Index) that extends the state-of-the-art index significantly by storing dynamic door-to-door distances in a compact distance cube associated with tree nodes. When processing ITSPQ using IT-Index, we make use of the distance cube to avoid time-consuming indoor distance computation on-the-fly. We evaluate the proposed techniques using extensive experiments on synthetic and real data. The results show that our IT-Index based method is the most efficient for processing ITSPQ at a modest cost of index memory consumption."
keywords:
  - "indoor"
  - "temporal"
  - "variation"
  - "aware"
  - "shortest"
  - "path"
  - "query"
  - "computer science"
  - "variation (astronomy)"
  - "query optimization"
doi: "10.1109/tkde.2021.3076144"
aliases:
  - "/en/publication/dblp-journalstkde-liu-fllccx-23/"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/tkde/LiuFLLCCX23"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
