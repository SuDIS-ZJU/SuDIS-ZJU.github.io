---
title: "FRAME: Feature rectification for class imbalance learning"
authors:
  - "Xu Cheng"
  - "Fan Shi"
  - "Yao Zhang"
  - "Huan Li"
  - "Xiufeng Liu"
  - "Shengyong Chen"
author_links:
  - name: "Huan Li"
    url: "/authors/huan-li/home/zh/"
date: "2024-01-01"
publishDate: "2024-01-01"
publication_types:
  - "paper-journal"
publication: "IEEE Transactions on Knowledge and Data Engineering (TKDE)"
venue: "IEEE Transactions on Knowledge and Data Engineering (TKDE)"
publication_kind: "journal"
slug: "paper-j013"
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "Class imbalance learning is a challenging task in ma- true in the real world, as the imbalance between classes can be chine learning applications. To balance training data, traditional widely observed [2]. For example, in building a machine learning class imbalance learning approaches, such as class resampling or model for cancer detection, the number of samples for healthy reweighting, are commonly applied in the literature. However, these methods can have significant limitations, particularly in people is much higher than that of “ill” people. Faced with the the presence of noisy data, missing values, or when applied to class imbalance problem, conventional machine learning models advanced learning paradigms like semi-supervised or federated usually form the so-called “majority bias”. ‘Majority bias’ refers learning. To address these limitations, this paper proposes a novel to the tendency of machine learning models to prioritize or and theoretically-ensured latent Feature Rectification method for favor the majority class over the minority class in imbalanced clAss iMbalance lEarning (FRAME). The proposed FRAME can automatically learn multiple centroids for each class in the latent datasets. This occurs because the model learns to minimize space and then perform class balancing. Unlike data-level meth- overall error, which can be achieved more easily by correctly ods, FRAME balances feature in the latent space rather than the predicting the majority class, often at the expense of the minority original space. Compared to algorithm-level methods, FRAME can class. This result is sub-optimal because the information from a distinguish different classes based on distance without the need to few majority classes is always concerned. adjust the learning algorithms. Through latent feature rectifica- tion, FRAME can effectively mitigate contaminated noises/missing To mitigate the issue of class imbalance, a variety of tradi- values without worrying about structural variations in the data. tional methods have been developed, classified into three main In order to accommodate a wider range of applications, this paper groups: data-level, algorithm-level, and ensemble methods [3]. extends FRAME to the following three main learning paradigms: Data-level techniques address the imbalance by either increas- fully-supervised learning, semi-supervised learning, and federated ing the instances of the minority class or decreasing those of learning. Extensive experiments on 10 binary-class datasets demon- strate that our FRAME can achieve competitive performance than the majority class [4]. Algorithm-level techniques adjust the the state-of-the-art methods and its robustness to noises/missing learning process to more effectively recognize features of the values. minority class [5]. Ensemble methods combine the power of"
keywords:
  - "frame"
  - "feature"
  - "rectification"
  - "class"
  - "imbalance"
  - "learning"
doi: "10.1109/tkde.2024.3523043"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/journals/tkde/ChengSZLLC25"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
