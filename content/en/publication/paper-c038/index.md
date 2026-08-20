---
title: "AlayaDB: The data foundation for efficient and effective long-context LLM inference"
authors:
  - "Yangsen Deng"
  - "[et al."
  - "including Huan Li]"
  - "and Bo Tang"
date: "2025-01-01"
publishDate: "2025-01-01"
publication_types:
  - "paper-conference"
publication: "2025 ACM SIGMOD International Conference on Management of Data (SIGMOD)"
venue: "2025 ACM SIGMOD International Conference on Management of Data (SIGMOD)"
publication_kind: "conference"
slug: "paper-c038"
design:
  css_class: single-language-section
venue_rankings:
  - "CCF-A"
  - "CORE-A*"
abstract: "These systems achieve high generation quality as they use a full AlayaDB is a cutting-edge vector database system natively archi- attention mechanism. Mooncake [51] and LMCache [15, 46] are [cs.AI] 14 Apr 2025 tected for efficient and effective long-context inference for Large representative LLM inference systems in (ii) KV cache disaggre- Language Models (LLMs) at AlayaDB AI. Specifically, it decouples gation. They store the KV cache of contexts in external storage the KV cache and attention computation from the LLM inference and reuse them among different LLM inference instances. Thus, systems, and encapsulates them into a novel vector database system. the inference latency of these systems is improved as it reuses For the Model as a Service providers (MaaS), AlayaDB consumes the KV cache and reduces the expensive computations (e.g., inner fewer hardware resources and offers higher generation quality for product and softmax). Recently, retrieval-based sparse attention various workloads with different kinds of Service Level Objectives solutions have been proposed (e.g., InfLLM [63] and RetrievalAt- (SLOs), when compared with the existing alternative solutions (e.g., tention [45]) to alleviate the large GPU memory consumption of KV cache disaggregation, retrieval-based sparse attention). The crux these systems in both (i) and (ii). The core idea behind them is the of AlayaDB is that it abstracts the attention computation and cache sparse attention mechanism, i.e., only a subset of critical key and management for LLM inference into a query processing procedure, value tokens are selected to perform the attention computation. and optimizes the performance via a native query optimizer. In this Unfortunately, existing systems cannot simultaneously optimize work, we demonstrate the effectiveness of AlayaDB via (i) two use the three aforementioned performance metrics, as we will elaborate cases from our industry partners, and (ii) extensive experimental in Section 3. results on LLM inference benchmarks. At AlayaDB.AI, we designed an LLM-native vector database AlayaDB to overcome the limitations of existing LLM inference CCS Concepts systems/solutions and enable efficient and effective long-context inference in LLM era. Specifically, for Model as a Service (MaaS) [38] • Information systems → Data management systems; • Com- providers, the SLOs of different kinds of workloads indicate their puting methodologies → Artificial intelligence. requirements for the inference latency. Thus, the core challenge of AlayaDB is solving a bi-objective optimization problem, i.e., meet"
keywords:
  - "alayadb"
  - "data"
  - "foundation"
  - "efficient"
  - "effective"
  - "long"
  - "context"
  - "llm"
  - "foundation (evidence)"
  - "inference"
doi: "10.1145/3722212.3724428"
links:
  - name: "DBLP"
    url: "https://dblp.org/rec/conf/sigmod/DengYXLYHZLLLMY25"
  - name: "arXiv"
    url: "https://arxiv.org/abs/2504.10326"
  - name: "Project"
    url: "https://longaspire.github.io/publication/"
---
