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
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-journal"
publication: "IEEE Transactions on Knowledge and Data Engineering (TKDE)"
slug: "paper-j016"
abstract: "Active learning (AL) reduces human annotation costs However, individual data owners performing AL often face for machine learning systems by strategically selecting the most constraints due to limited human resources and the isolated informative unlabeled data for annotation, but performing it in- nature of data samples, which can hinder achieving satisfac- dividually may still be insufficient due to restricted data diver- sity and annotation budget. Federated Active Learning (FAL) ad- tory model accuracy. The ideal solution involves collaborative dresses this by facilitating collaborative data selection and model efforts from multiple data owners in annotation and training [4], training, while preserving the confidentiality of raw data samples. [5]. However, such collaboration raises concerns regarding data Yet, existing FAL methods fail to account for the heterogeneity privacy, as direct sharing of raw data for annotation and training of data distribution across clients and the associated fluctuations may not always be feasible or appropriate. in global and local model parameters, adversely affecting model accuracy. To overcome these challenges, we propose CHASe (Client Federated Learning (FL) [6], [7], [8], [9], [10] has been Heterogeneity-Aware Data Selection), specifically designed for proposed for conducting machine learning in a decentralized FAL. CHASe focuses on identifying those unlabeled samples with manner by communicating the parameters instead of raw data. high epistemic variations (EVs), which notably oscillate around the The main idea is to obtain a global shared model by aggregating decision boundaries during training. To achieve both effectiveness models trained locally on the distributed clients [11]. Driven by and efficiency, CHASe encompasses techniques for 1) tracking EVs by analyzing inference inconsistencies across training epochs, 2) the potential benefits of leveraging other clients’ data and an- calibrating decision boundaries of inaccurate models with a new notation capabilities, the concept of Federated Active Learning alignment loss, and 3) enhancing data selection efficiency via a data (FAL) is emerging. In FAL, each client performs AL to annotate freeze and awaken mechanism with subset sampling. Experiments its data, trains a local model with newly labeled data, and show that CHASe surpasses various established baselines in terms sends its model update to a central server to obtain a consensus of effectiveness and efficiency, validated across diverse datasets, model complexities, and heterogeneous federation settings. model. In traditional FAL, data selection spans the entire FL training cycle [12], [13], [14]. Here, we focus on scenarios where"
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
