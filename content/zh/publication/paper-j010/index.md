---
title: "Worker-churn-based task assignment with context-LSTM in spatial crowdsourcing"
authors:
  - "Yan Zhao"
  - "Tinghao Lai"
  - "Ziwei Wang"
  - "Kaixuan Chen"
  - "李环"
  - "Kai Zheng"
date: "2023-01-01"
publishDate: "2023-01-01"
publication_types:
  - "paper-journal"
publication: "IEEE Transactions on Knowledge and Data Engineering (TKDE)"
slug: "paper-j010"
abstract: "The pervasiveness of GPS-enabled devices and wire- and Wikipedia.2 Along with the ubiquity of GPS-equipped net- less communication technologies flourish the market of Spatial worked devices, e.g., smartphones, a new class of crowdsourc- Crowdsourcing (SC), which consists of location-based tasks and requires workers to be at specific locations physically to complete ing, called Spatial Crowdsourcing (SC), has drawn increasing them. In this work, we study the problem of worker-churn-based attention in both academia and industry. With SC, requesters can task assignment in SC, where tasks are assigned by considering issue spatial tasks (e.g., monitoring traffic conditions and picking workers’ churn. In particular, we aim to maximize the total rewards up passengers) to SC servers that then assign workers to these of task assignments based on the worker churn prediction. To solve tasks (called task assignment). Workers complete their tasks by the problem, we propose a two-phase framework, which consists of a worker churn prediction and a task assignment phase. In moving to the specified locations. Spatio-temporal information the first phase, we use an LSTM-based model to extract latent (e.g., location, mobility, and the associated contexts) plays a feelings of workers based on historical data and then estimate idle crucial role in SC. Due to its natural connection to the physical time intervals of workers. In the assignment phase, we design an world, SC is relevant to a wide spectrum of daily applications, efficient greedy algorithm and a Kuhn-Munkras-based algorithm including real-time ride-hailing services (e.g., Uber3 ), and on- that can achieve the optimal task assignment. To improve the accuracy of the idle time interval estimation for workers, we adopt wheel meal-ordering services (e.g., GrubHub4 ). a context-dependent LSTM model, which involves interactions Research on SC [6], [7], [8], [11], [38], [41], [44], [45], [47], between inputs and their context. We further optimize the original [48], [49], [50], [51] has gained momentum in recent years; con- task assignment framework by proposing a travel distance opti- sequently, many techniques of task assignment are proposed for mization strategy to reduce the overall travel distance. Extensive different application scenarios. Cheng et al. [10] study a reliable experiments offer insight into the effectiveness and efficiency of the proposed solutions. diversity-based spatial crowdsourcing (RDB-SC) problem in SC, which aims to maximize the diversity score of assignments."
keywords:
  - "worker"
  - "churn"
  - "task"
  - "assignment"
  - "context"
  - "lstm"
  - "spatial"
  - "crowdsourcing"
doi: "10.1109/tkde.2023.3249828"
aliases:
  - "/zh/publication/dblp-journalstkde-zhao-lwclz-23/"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/tkde/ZhaoLWCLZ23"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
