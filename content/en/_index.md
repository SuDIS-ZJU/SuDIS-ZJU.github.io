---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: markdown
    content:
      title: 'SuDIS@ZJU'
      subtitle: ''
      text: |
        **Data Drives, Efficiency Defines, Together We Compute.**

        SuDIS is the Sustainable Data Intelligence and Data Systems research group at Zhejiang University. We study how data quality, efficient models, and data systems can work together to make intelligent applications scalable, reliable, and deployable.

        **Core directions:** Data-centric AI · Efficient AI · Data Systems for AI

        *Rapid · Reliable · Responsible · Resilient*
    design:
      columns: '1'
      background:
        image:
          filename: group.jpg
          filters:
            brightness: 0.4
          parallax: true
          position: center
          size: cover
          text_color_light: true
      spacing:
        padding: ['220px', '0', '220px', '0']
      css_class:

  - block: markdown
    content:
      title: Our Vision
      text: |
        SuDIS is a research group at Zhejiang University dedicated to resource-efficient, data-centric artificial intelligence and the data systems that make intelligent services reliable, scalable, and deployable. We investigate AI data preparation and quality governance, efficient inference and serving for large and multimodal models, spatiotemporal intelligence, model and system lightweighting, and data management for emerging LLM- and agent-driven workloads. Our work has appeared in SIGMOD, VLDB, KDD, WWW, NeurIPS, ICML, ICLR, ACL, and related venues, and is carried out with partners including Alibaba Cloud (ATH, PAI, and Database), Ant Group (healthcare, security, and computing platforms), Baidu's foundation-model team, Tencent, ByteDance, Xiaohongshu, and OPPO. We train PhD and master's students, undergraduate researchers, postdoctoral researchers, and interns through close mentorship and end-to-end research practice, supported by National Natural Science Foundation key, overseas-young-scholar, and young-scientist grants, National Key R&D Program young-scientist and major-subproject support, Zhejiang provincial major natural-science and Pioneer programs, and more than ten industry collaborations. We welcome students and interns who want to turn data intelligence and efficient computing into dependable systems with lasting scientific and societal value.
    design:
      columns: '1'

  - block: collection
    content:
      title: Latest News
      subtitle:
      text:
      count: 4
      filters:
        author: ''
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: ''
      offset: 0
      order: desc
      page_type: post
    design:
      view: card
      columns: '1'

  - block: collection
    content:
      title: Latest Publications
      text: ""
      count: 3
      filters:
        folders:
          - publication
    design:
      view: citation
      columns: '1'

  - block: markdown
    content:
      title: Research, Projects and Training
      text: |
        SuDIS develops resource-efficient, data-centric AI and the systems that support it. Current work spans multimodal data quality, large-model inference and serving, data preparation, time-series intelligence, and next-generation data management. We connect rigorous research with open-source artifacts, real workloads, and responsible deployment, giving students and interns a complete path from problem formulation to reproducible systems and public communication.

        Our public project portfolio highlights selected national, university, and industry collaborations. Project cards expose only the public project name, partner/source, and active period.

        <!-- PUBLIC_PROJECTS_EN_BEGIN -->
        | Project | Source | Period |
        |---|---|---|
        | Continual post-training systems for reasoning models on domestic intelligent-computing platforms | National Key R&D Program | 2026–2029 |
        | Theory and methods for structured big-data foundation models | National research program | 2025–2028 |
        | Zhejiang University–Ant Joint Research Center for Big-Data Cognitive Computing | Ant Group | 2025–2028 |
        | Multimodal data governance for large-model training | Zhejiang Provincial Major Program | 2024–2026 |
        | Data preparation, optimization, and augmentation for domain large models | Zhejiang Provincial Innovation Program | 2024–2026 |
        | Data quality for IoT intelligence | National Natural Science Foundation | 2023–2026 |
        | Multimodal data intelligence for new-energy vehicles | Industry collaboration | 2025–2028 |
        | Continuous profiling for MoE inference optimization | CCF–Ant Research Fund | 2026–2027 |
        | Efficient inference for multimodal ultra-long sequences | CCF–Baidu Research Fund | 2025–2026 |
        | OLAP multi-tenant isolation and runtime resource optimization | CCF–Alibaba Cloud Research Fund | 2024–2025 |
        | AI-enabled chronic disease management | National research program | 2026–2030 |
        | Personalized medical agents with memory layers | Industry collaboration | 2026–2027 |
        | Key technologies for edge-intelligent time-series imputation | National Natural Science Foundation | 2025–2027 |
        | Real-time big-data technology for modern industrial systems | Ministry of Education teaching case | 2025–2026 |
        <!-- PUBLIC_PROJECTS_EN_END -->
    design:
      columns: '1'

  - block: markdown
    content:
      title: Join Us
      text: |
        We welcome doctoral students, postdoctoral researchers, research assistants, and undergraduate interns interested in:

        - LLM, multimodal LLM, and agentic inference optimization
        - Data preparation and quality governance for domain models
        - Data systems for multimodal, decentralized, and LLM-driven workloads
        - Intelligent computing for spatiotemporal data

        The group supports research exchange and project practice with leading universities and technology companies.
    design:
      columns: '1'

  - block: markdown
    content:
      title:
      subtitle:
      text: |
        {{% cta cta_link="./people/" cta_text="Meet the team →" %}}
    design:
      columns: '1'
---
