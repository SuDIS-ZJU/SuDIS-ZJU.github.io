---
title: "FedBFPT: An efficient federated learning framework for Bert further pre-training"
authors:
  - "Xin'ao Wang"
  - "Huan Li"
  - "Ke Chen"
  - "Lidan Shou"
author_links:
  - name: "Xin'ao Wang"
    url: "/authors/xin-ao-wang/home/"
  - name: "Huan Li"
    url: "/authors/huan-li/home/"
date: "2023-01-01"
publishDate: "2023-01-01"
publication_types:
  - "paper-conference"
publication: "The 32nd International Joint Conference on Artificial Intelligence (IJCAI)"
venue: "The 32nd International Joint Conference on Artificial Intelligence (IJCAI)"
publication_kind: "conference"
slug: "paper-c022"
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "al., 2018], GPT [Radford et al., 2018], BERT [Devlin et al., 2019], and RoBERTa [Liu et al., 2019]. These models This study proposes F ED BFPT (Federated BERT are typically trained on general corpora but can yield better Further Pre-Training), a Federated Learning (FL) performance on specialized domain tasks after undergoing framework for further pre-training the BERT lan- further pre-training [Beltagy et al., 2019] using specialized guage model in specialized domains while address- datasets. However, collecting such specialized datasets cen- ing privacy concerns. F ED BFPT enables multiple trally poses privacy concerns, making it infeasible. clients to collaboratively train the shallower lay- Previous research has shown that neural networks tend ers of BERT, which are crucial in the pre-training to stabilize from shallower to deeper layers during train- stage, without the need to share private data. To ing [Raghu et al., 2017]. This has been observed in the popu- achieve this, F ED BFPT involves building a lo- lar pre-trained language model BERT, where shallower layers cal model for each client, progressively training have been shown to capture phrase-level information, which the shallower layers of local models while sam- holds greater significance in model pre-training compared to pling deeper layers, and aggregating trained pa- the deeper layers [Jawahar et al., 2019; Hao et al., 2019; rameters on a server to create the final global Manginas et al., 2020; Wang et al., 2022b]. The observa- model. This approach utilizes multiple smaller tion suggests that it might be feasible to train only a subset local models to further pre-train a global model of layers on the client side initially and gradually increase the targeted at specific tasks via fine-tuning, resulting number of trained layers, thereby achieving efficient training in a reduction in resource usage while maintain- of large models in an FL setting. ing model accuracy. Theoretical analysis is con- In this paper, we focus on the cost-effectiveness of BERT’s ducted to support the efficiency of F ED BFPT, and pre-training in FL by asking the following questions: (1) experiments are conducted on corpora across do- Can we design a computational and communication efficient mains such as medicine, biology, and computer method to complete the training of large models in resource- science. Results indicate that F ED BFPT achieves constrained clients? (2) Can such a method achieve the accu- performance levels comparable to traditional FL racy of traditional FL or even centralized training? methods while reducing computation and commu- nication costs by 46.70% and 7.04%, respectively, Our answers to both questions are ”Yes.” Through investi- even approaching the performance of centralized gation, we propose F ED BFPT (Federated BERT Further Pre- training models. The Source code is released at Training), an efficient framework that trains only part of the https://github.com/Hanzhouu/FedBFPT. layers of BERT to reduce the computational and communica- tion costs. F ED BFPT allows for training a large global model using FL by creating small local models for each client to"
keywords:
  - "fedbfpt"
  - "efficient"
  - "federated"
  - "learning"
  - "framework"
  - "bert"
  - "further"
  - "pre"
doi: "10.24963/ijcai.2023/483"
aliases:
  - "/en/publication/dblp-confijcai-wang-00-s-23/"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/ijcai/Wang00S23"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
