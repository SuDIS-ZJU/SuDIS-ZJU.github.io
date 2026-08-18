---
title: "Towards crowd-aware indoor path planning"
authors:
  - "Tiantian Liu"
  - "Huan Li"
  - "Hua Lu"
  - "Muhammad Aamir Cheema"
  - "Lidan Shou"
date: "2021-01-01"
publishDate: "2021-01-01"
publication_types:
  - "paper-conference"
publication: "The 47th International Conference on Very Large Data Bases (VLDB)"
slug: "paper-c012"
abstract: "path with fewer people en route to mitigate the interference and [cs.DB] 29 Apr 2021 Indoor venues accommodate many people who collectively form inconvenience caused by contact with people. crowds. Such crowds in turn influence people’s routing choices, In this paper, we formulate and study two crowd-aware indoor e.g., people may prefer to avoid crowded rooms when walking path planning queries. Referring to Figure 1, given a source point 𝑝𝑠 , from A to B. This paper studies two types of crowd-aware indoor a target point 𝑝𝑡 , and a query time 𝑡, an Indoor Crowd-Aware Fastest path planning queries. The Indoor Crowd-Aware Fastest Path Path Query (FPQ) returns a path with the shortest travel time in the Query (FPQ) finds a path with the shortest travel time in the presence of crowds, whereas an Indoor Least Crowded Path Query presence of crowds, whereas the Indoor Least Crowded Path Query (LCPQ) returns a path that encounters the least objects en route. (LCPQ) finds a path encountering the least objects en route. To As an indoor path is essentially a series of indoor partitions (basic process the queries, we design a unified framework with three topological units like rooms), FPQ’s routing cost is partition-passing major components. First, an indoor crowd model organizes indoor time, whereas an LCPQ’s is partition-passing contact. topology and captures object flows between rooms. Second, a time- (4, 6, 0) (20, 120, 15) ps d5 evolving population estimator derives room populations for a future d2 (4, 6, 0) (5, 12, 2) timestamp to support crowd-aware routing cost computations in d1 (8, 12, 0) d8 query processing. Third, two exact and two approximate query d3 (20, 72, 2) (3, 6, 1) (3, 6, 1) processing algorithms process each type of query. All algorithms d6 Pt (3, 6, 1) are based on graph traversal over the indoor crowd model and use (16, 24, 0) d9 d4 (20, 30, 2) d7 (5, 12, 2) the same search framework with different strategies of updating the (distance, time populations during the search process. All proposals are evaluated v1 v3 v6 cost, contact) experimentally on synthetic and real data. The experimental results ps d5 d1 demonstrate the efficiency and scalability of our framework and d2 d4 doors d1 query processing algorithms. d8 door v2 Pt directionality d3 v4 d6 v7 v1 R-partition d9 v4 Q-partition"
keywords:
  - "crowd"
  - "aware"
  - "indoor"
  - "path"
  - "planning"
doi: "10.14778/3457390.3457401"
aliases:
  - "/en/publication/dblp-journalspvldb-liu-llcs-21/"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/pvldb/LiuLLCS21"
  - name: "arXiv"
    url: "https://arxiv.org/abs/2104.05480"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
