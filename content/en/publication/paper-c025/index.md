---
title: "Preventing the popular item embedding based attack in federated recommendations"
authors:
  - "Jun Zhang"
  - "Huan Li"
  - "Dazhong Rong"
  - "Yan Zhao"
  - "Ke Chen"
  - "Lidan Shou"
date: "2023-01-01"
publishDate: "2023-01-01"
publication_types:
  - "paper-conference"
publication: "The 40th IEEE International Conference on Data Engineering (ICDE)"
slug: "paper-c025"
abstract: "Privacy concerns have led to the rise of federated recommendation lists. Although these tactics may seem neg- recommender systems (FRS), which can create personalized ligible due to the minor impact on model performance, they models across distributed clients. However, FRS is vulnerable to inﬂict more harm on users than those untargeted attacks (only poisoning attacks, where malicious users manipulate gradients to promote their target items intentionally. Existing attacks against aiming for performance degradation) [4], [10], [18]. FRS have limitations, as they depend on speciﬁc models and User Embedding Historical prior knowledge, restricting their real-world applicability. In our MF-FRS Approximation Interactions exploration of practical FRS vulnerabilities, we devise a model- Federated Item Popularity agnostic and prior-knowledge-free attack, named P IECK (Popu- Recommender fx Item Popularity Enhancement System lar Item Embedding based Attack). The core module of P IECK is Interaction Function DL-FRS popular item mining, which leverages embedding changes during Poisoning Prior Knowledge FRS training to effectively identify the popular items. Built upon fx :Interaction Function :Fixed Dot Product :Learnable Parameters the core module, P IECK branches into two diverse solutions: The P IECK I PE solution employs an item popularity enhancement Fig. 1: Targeted model poisoning attacks against FRS. module, which aligns the embeddings of targeted items with the mined popular items to increase item exposure. The P IECK U EA Fig. 1 provides an overall picture of targeted poisoning at- further enhances the robustness of the attack by using a user tacks. Two main types of FRS exist: matrix factorization-based embedding approximation module, which approximates private FRS (MF-FRS) and deep learning-based FRS (DL-FRS). user embeddings using mined popular items. Upon identifying Interaction function poisoning [30] based attacks exclusively P IECK, we evaluate existing federated defense methods and ﬁnd them ineffective against P IECK, as poisonous gradients inevitably target DL-FRS with an assumption that a learnable interaction overwhelm the cold target items. We then propose a novel defense function exists2 . While the other attacks based on user embed- method by introducing two regularization terms during user ding approximation [31] or item popularity enhancement [41] training, which constrain item popularity enhancement and user are model-agnostic, they assume prior knowledge of historical embedding approximation while preserving FRS performance. user-item interaction data or item popularity levels. These We evaluate P IECK and its defense across two base models, three real datasets, four top-tier attacks, and six general defense assumptions, practically inapplicable (no sense to provide such methods, afﬁrming the efﬁcacy of both P IECK and its defense. information to attackers), do not lend the corresponding attacks"
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
