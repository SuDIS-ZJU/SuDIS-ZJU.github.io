---
title: "Towards crowd-aware indoor path planning"
authors:
  - "Tiantian Liu"
  - "Huan Li"
  - "Hua Lu"
  - "Muhammad Aamir Cheema"
  - "Lidan Shou"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2021-01-01"
publishDate: "2021-01-01"
publication_types:
  - "paper-conference"
publication: "The 47th International Conference on Very Large Data Bases (VLDB)"
venue: "The 47th International Conference on Very Large Data Bases (VLDB)"
publication_kind: "conference"
slug: "paper-c012"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "Indoor venues accommodate many people who collectively form crowds. Such crowds in turn influence people’s routing choices, e.g., people may prefer to avoid crowded rooms when walking from A to B. This paper studies two types of crowd-aware indoor path planning queries. The Indoor Crowd-Aware Fastest Path Query (FPQ) finds a path with the shortest travel time in the presence of crowds, whereas the Indoor Least Crowded Path Query (LCPQ) finds a path encountering the least objects en route. To process the queries, we design a unified framework with three major components. First, an indoor crowd model organizes indoor topology and captures object flows between rooms. Second, a timeevolving population estimator derives room populations for a future timestamp to support crowd-aware routing cost computations in query processing. Third, two exact and two approximate query processing algorithms process each type of query. All algorithms are based on graph traversal over the indoor crowd model and use the same search framework with different strategies of updating the populations during the search process. All proposals are evaluated experimentally on synthetic and real data. The experimental results demonstrate the efficiency and scalability of our framework and query processing algorithms."
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
