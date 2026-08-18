---
title: "TRIPS: A system for translating raw indoor positioning data into visual mobility semantics"
authors:
  - "Huan Li"
  - "Hua Lu"
  - "Feichao Shi"
  - "Gang Chen"
  - "Ke Chen"
  - "Lidan Shou"
date: "2018-01-01"
publishDate: "2018-01-01"
publication_types:
  - "paper-conference"
publication: "The 44th International Conference on Very Large Data Bases (VLDB)"
slug: "paper-c002"
abstract: "analyst for a shopping mall needs to know if a shopper has stayed The rapid accumulation of indoor positioning data is increasingly in a shop for a period of time sufficiently long for a real purchase. booming the interest in indoor mobility analyses. As a fundamen- In such a case, it is insufficient to only look at the raw position- tal analysis, it is highly relevant to translate raw indoor positioning ing records; some richer and more comprehensible annotations are data into mobility semantics that describe what, where and when in needed as semantics. To this end, the analyst can configure the re- a more concise and semantics-oriented way. Such a translation is lated contexts that help to determine the annotations. In particular, challenging as multiple data sources are involved, raw indoor po- she may specify the regions for all shops (e.g., a Nike Store) in the sitioning data is of low quality, and translation results are hard to mall and define a pattern of mobility event that someone stays in assess. We demonstrate a system TRIPS that streamlines the entire one or multiple shops. Given such contexts, the raw data can be translation process by three functional components. The Configu- translated into a high-level representation that is more concise and rator provides a standard but concise means to configure multiple readable. An example is given in the right part of Table 1. input sources, including the indoor positioning data, indoor space Table 1: Raw Indoor Positioning Data vs. Mobility Semantics information, and relevant contexts. The Translator cleans the in- door positioning data and exports reliable mobility semantics with- Raw Positioning Records Mobility Semantics out manual interventions. The Viewer offers a suite of flexible op- oi , (5.1, 12.7, 3F ), 1:02:05pm oi : erations to trace the input, output and intermediate data involved in oi , (6.5, 11.8, 3F ), 1:02:12pm (stay, Adidas, 1:02:05-1:18:15pm) the translation. Data analysts can interact with TRIPS to obtain the ......... (pass-by, Nike, 1:18:16-1:20:13pm) oi , (13.6, 4.2, 2F ), 1:24:05pm (stay, Cashier, 1:20:14-1:24:05pm) desired mobility semantics in a visual and convenient way. PVLDB Reference Format: In this example, a shopper oi ’s mobility behaviors are described Huan Li, Hua Lu, Feichao Shi, Gang Chen, Ke Chen and Lidan Shou. by a sequence of triplets called mobility semantics. Each triplet in- TRIPS: A System for Translating Raw Indoor Positioning Data into Visual cludes an event annotation (mobility event stay or pass-by), a spa- Mobility Semantics. PVLDB, 11 (12): 1918-1921, 2018. tial annotation (a semantic region like Nike Store) and a temporal DOI: https://doi.org/10.14778/3229863.3236224 annotation (time period). In our definition, a mobility event refers to a generic movement pattern of some particular interest, and a 1."
keywords:
  - "trips"
  - "system"
  - "translating"
  - "raw"
  - "indoor"
  - "positioning"
  - "data"
  - "visual"
doi: "10.14778/3229863.3236224"
aliases:
  - "/en/publication/dblp-journalspvldb-li-lsccs-18/"
links:
  - name: "DOI"
    url: "https://doi.org/10.14778/3229863.3236224"
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/pvldb/LiLSCCS18"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
