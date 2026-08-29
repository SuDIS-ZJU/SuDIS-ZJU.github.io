---
title: "CHASe: Client heterogeneity-aware data selection for effective federated active learning"
authors:
  - "Jun Zhang"
  - "Jue Wang"
  - "Huan Li"
  - "Zhongle Xie"
  - "Ke Chen"
  - "Lidan Shou"
author_links:
  - name: "Jun Zhang"
    url: "/authors/jun-zhang/home/"
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-journal"
publication: "IEEE Transactions on Knowledge and Data Engineering (TKDE)"
venue: "IEEE Transactions on Knowledge and Data Engineering (TKDE)"
publication_kind: "journal"
slug: "paper-j016"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "Active learning (AL) reduces human annotation costs for machine learning systems by strategically selecting the most informative unlabeled data for annotation, but performing it individually may still be insufficient due to restricted data diversity and annotation budget. Federated Active Learning (FAL) addresses this by facilitating collaborative data selection and model training, while preserving the confidentiality of raw data samples. Yet, existing FAL methods fail to account for the heterogeneity of data distribution across clients and the associated fluctuations in global and local model parameters, adversely affecting model accuracy. To overcome these challenges, we proposeCHASe (Client Heterogeneity-Aware Data Selection), specifically designed for FAL. CHASe focuses on identifying those unlabeled samples with high epistemic variations (EVs), which notably oscillate around the decision boundaries during training. To achieve both effectiveness and efficiency, CHASe encompasses techniques for 1) tracking EVs by analyzing inference inconsistencies across training epochs, 2) calibrating decision boundaries of inaccurate models with a new alignment loss, and 3) enhancing data selection efficiency via a data freeze and awaken mechanism with subset sampling. Experiments show that CHASe surpasses various established baselines in terms of effectiveness and efficiency, validated across diverse datasets, model complexities, and heterogeneous federation settings."
keywords:
  - "chase"
  - "client"
  - "heterogeneity"
  - "aware"
  - "data"
  - "selection"
  - "effective"
  - "federated"
doi: "10.1109/tkde.2025.3547423"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/tkde/ZhangWLXCS25"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
