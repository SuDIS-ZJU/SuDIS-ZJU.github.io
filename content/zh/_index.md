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
        **数据为舟，效率为帆，共赴计算之海。**

        SuDIS 是浙江大学可持续数据智能与数据系统课题组，聚焦数据质量、高效模型与数据系统的协同，推动人工智能走向可扩展、可靠和可落地。

        **核心方向：** Data-centric AI · Efficient AI · Data Systems for AI

        *快速 · 可靠 · 负责 · 弹性*
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
      title: 团队愿景
      text: |
        SuDIS 是浙江大学面向数据智能与数据系统的研究团队，致力于研究资源高效、以数据为中心的人工智能方法，以及支撑智能服务可靠、可扩展和可部署的数据系统。我们聚焦人工智能数据准备与质量治理、大模型与多模态模型的高效推理和部署、时空智能、模型与系统轻量化，以及面向大模型和智能体工作负载的新型数据管理。团队成果发表于 SIGMOD、VLDB、KDD、WWW、NeurIPS、ICML、ICLR、ACL 等国际会议和期刊，并与阿里云（ATH、PAI、数据库）、蚂蚁集团（大健康、大安全、计算平台）、百度大模型部、腾讯、字节跳动、小红书、OPPO 等合作伙伴开展研究。我们通过持续指导和端到端科研实践培养博士生、硕士生、本科生、博士后与实习生，承担国家自然科学基金重点项目、海外优青和青年项目，国家重点研发计划青年科学家项目及重大专项子课题，浙江省重大自然科学基金和尖兵项目，并已开展十余项蚂蚁、阿里云、百度等企业横向合作。我们诚邀希望在数据智能与高效计算前沿开展严谨研究、构建可复现系统并产生长期学术与社会价值的同学和实习生加入 SuDIS。
    design:
      columns: '1'

  - block: collection
    content:
      title: 近期动态
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
      title: 最新成果
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
      title: 研究、项目与人才培养
      text: |
        SuDIS 研究资源高效、以数据为中心的人工智能，以及支撑人工智能规模化应用的数据系统。当前工作覆盖多模态数据质量、大模型推理与部署、领域数据准备、时间序列智能计算和新型数据管理系统，并将严谨问题定义、开源实现、真实工作负载与负责任部署贯通起来，为学生和实习生提供从研究问题到可复现系统和公开成果的完整培养路径。

        首页项目区精选国家项目、校企合作和公开研究项目，只展示公开项目名称、合作来源和项目周期。

        <!-- PUBLIC_PROJECTS_ZH_BEGIN -->
        | 项目 | 来源 | 周期 |
        |---|---|---|
        | 面向国产智算平台的推理模型持续后训练系统 | 国家重点研发计划 | 2026–2029 |
        | 结构化大数据元模型构建理论与方法研究 | 国家重点项目 | 2025–2028 |
        | 浙大—蚂蚁大数据认知计算联合研究中心 | 蚂蚁集团 | 2025–2028 |
        | 面向大模型训练的多模态数据治理策略研究 | 浙江省重大基金 | 2024–2026 |
        | 面向领域大模型的数据准备、优化与增广 | 浙江省尖兵计划 | 2024–2026 |
        | 物联网智能计算中的数据质量 | 国家自然科学基金 | 2023–2026 |
        | 新能源车企多模态数据智能服务 | 校企合作 | 2025–2028 |
        | 面向 MoE 大模型推理优化的 Continuous Profiling | CCF—蚂蚁科研基金 | 2026–2027 |
        | 稀疏注意力驱动的多模态超长序列高效推理 | CCF—百度松果基金 | 2025–2026 |
        | OLAP 多租任务隔离与运行资源优化 | CCF—阿里云瑶池基金 | 2024–2025 |
        | 人工智能赋能慢病防治管理新范式研究 | 国家科技重大专项 | 2026–2030 |
        | 基于记忆层的个体化医疗 Agent 研究 | 产业合作 | 2026–2027 |
        | 边缘智能时序数据插补关键技术研究 | 国家自然科学基金 | 2025–2027 |
        | 实时大数据技术引领现代化产业体系升级 | 教育部主题案例 | 2025–2026 |
        <!-- PUBLIC_PROJECTS_ZH_END -->
    design:
      columns: '1'

  - block: markdown
    content:
      title: 加入我们
      text: |
        团队长期开放博士后、科研助理和本科生实习岗位，欢迎关注以下方向：

        - 大模型、多模态大模型与智能体推理优化
        - 领域大模型数据准备与质量治理
        - 面向多模态、去中心化和大模型工作负载的数据系统
        - 时空大数据智能计算

        团队支持成员参与国内外高校学术交流及产业项目实践。
    design:
      columns: '1'

  - block: markdown
    content:
      title:
      subtitle:
      text: |
        {{% cta cta_link="/en/people/" cta_text="团队成员 →" %}}
    design:
      columns: '1'
---
