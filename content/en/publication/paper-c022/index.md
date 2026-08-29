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
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "This study proposes FEDBFPT (Federated BERT Further Pre-Training), a Federated Learning (FL) framework for further pre-training the BERT language model in specialized domains while addressing privacy concerns. FEDBFPT enables multiple clients to collaboratively train the shallower layers of BERT, which are crucial in the pre-training stage, without the need to share private data. To achieve this, FEDBFPT involves building a local model for each client, progressively training the shallower layers of local models while sampling deeper layers, and aggregating trained parameters on a server to create the final global model. This approach utilizes multiple smaller local models to further pre-train a global model targeted at specific tasks via fine-tuning, resulting in a reduction in resource usage while maintaining model accuracy. Theoretical analysis is conducted to support the efficiency of FEDBFPT, and experiments are conducted on corpora across domains such as medicine, biology, and computer science. Results indicate that FEDBFPT achieves performance levels comparable to traditional FL methods while reducing computation and communication costs by 46.70% and 7.04%, respectively, even approaching the performance of centralized training models. The Source code is released at https://github.com/Hanzhouu/FedBFPT."
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
