---
title: "Vita: A versatile toolkit for generating indoor mobility data for real-world buildings"
authors:
  - "李环"
  - "Hua Lu"
  - "Xin Chen"
  - "Gang Chen"
  - "Ke Chen"
  - "Lidan Shou"
date: "2018-01-01"
publishDate: "2018-01-01"
publication_types:
  - "paper-conference"
publication: "The 42nd International Conference on Very Large Data Bases (VLDB)"
slug: "paper-c003"
abstract: "In order to support relevant studies, we need a versatile data We demonstrate a generic, user-configurable toolkit for generating generator that is able to generate various indoor mobility data different types of indoor mobility data for real-world buildings. according to user needs. Such a generator can be used for two Our prototype generates the desired data in a three-layer pipeline. purposes: (1) It can be used to generate mobility data, which is The Infrastructure Layer accepts industry-standard digital building typically given as a discrete sequence of user location estimates. information (DBI) files to generate the host indoor environment, al- (2) It can provide the “ground truth” for the mobility data generated lowing users to configure the generation of a variety of positioning in (1), to evaluate the models/algorithms being studied. For exam- devices, such as Wi-Fi, Bluetooth, RFID, etc. The Moving Object ple, a data generator can preserve the underlying raw trajectory Layer offers the functionality of defining objects or trajectories, while generating the corresponding synthetic indoor positioning with configurable indoor moving patterns, distribution models, and data. Particularly, the former can be preserved in a fine temporal sampling frequencies. The Positioning Layer generates synthetic granularity, whereas the latter can be set according to a lower signal strength measurements known as raw RSSI1 measurements sampling frequency to simulate a real indoor positioning system. according to the positioning device data and trajectory data gener- In this sense, such a data generator can provide “ground truth” ated at relevant layers. It also generates different types of indoor indoor movement data, which is indispensable for effectiveness positioning data through the customization of all typical indoor evaluations needed by mining and analytics. Such ground truth positioning methods on the raw RSSI data. is usually missing in real indoor positioning data due to the low sampling frequency and/or low accuracy. Consequently, an object’s whereabout is unknown between two consecutive reported 1."
keywords:
  - "vita"
  - "versatile"
  - "toolkit"
  - "generating"
  - "indoor"
  - "mobility"
  - "data"
  - "real"
doi: "10.14778/3007263.3007282"
aliases:
  - "/zh/publication/dblp-journalspvldb-li-lcccs-16/"
links:
  - name: "DOI"
    url: "https://doi.org/10.14778/3007263.3007282"
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/pvldb/LiLCCCS16"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
