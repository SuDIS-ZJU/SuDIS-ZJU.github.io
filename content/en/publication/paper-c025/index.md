---
title: "Preventing the popular item embedding based attack in federated recommendations"
authors:
  - "Jun Zhang"
  - "Huan Li"
  - "Dazhong Rong"
  - "Yan Zhao"
  - "Ke Chen"
  - "Lidan Shou"
author_links:
  - name: "Jun Zhang"
    url: "/authors/jun-zhang/home/"
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2023-01-01"
publishDate: "2023-01-01"
publication_types:
  - "paper-conference"
publication: "The 40th IEEE International Conference on Data Engineering (ICDE)"
venue: "The 40th IEEE International Conference on Data Engineering (ICDE)"
publication_kind: "conference"
slug: "paper-c025"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "Privacy concerns have led to the rise of federated recommender systems (FRS), which can create personalized models across distributed clients. However, FRS is vulnerable to poisoning attacks, where malicious users manipulate gradients to promote their target items intentionally. Existing attacks against FRS have limitations, as they depend on specific models and prior knowledge, restricting their real-world applicability. In our exploration of practical FRS vulnerabilities, we devise a modelagnostic and prior-knowledge-free attack, named PIECK (Popular Item Embedding based Attack). The core module of PIECK is popular item mining, which leverages embedding changes during FRS training to effectively identify the popular items. Built upon the core module, PIECK branches into two diverse solutions: The PIECKIPE solution employs an item popularity enhancement module, which aligns the embeddings of targeted items with the mined popular items to increase item exposure. The PIECKUEA further enhances the robustness of the attack by using a user embedding approximation module, which approximates private user embeddings using mined popular items. Upon identifying PIECK, we evaluate existing federated defense methods and find them ineffective against PIECK, as poisonous gradients inevitably overwhelm the cold target items. We then propose a novel defense method by introducing two regularization terms during user training, which constrain item popularity enhancement and user embedding approximation while preserving FRS performance. We evaluate PIECK and its defense across two base models, three real datasets, four top-tier attacks, and six general defense methods, affirming the efficacy of both PIECK and its defense."
keywords:
  - "preventing"
  - "popular"
  - "item"
  - "embedding"
  - "attack"
  - "federated"
  - "recommendations"
doi: "10.1109/icde60146.2024.00173"
aliases:
  - "/en/publication/dblp-conficde-zhang-0-rz-0-s-24/"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/icde/Zhang0RZ0S24"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
