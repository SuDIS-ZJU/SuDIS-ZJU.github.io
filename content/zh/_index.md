---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  # - block: hero
  #   content:
  #     title: |
  #       👋 Hello
  #     image:
  #       filename: welcome.jpg
  #     text: |
  #
  #       Welcome to **SuDIS** --- the *Sustainable Data Intelligence and Data Systems* research group at Zhejiang University, where we hack on making data smarter and systems stronger. We explore modern architectures and algorithms to achieve **Rapid, Reliable, Responsible, and Resilient** solutions that tackle real-world problems. If you’re as passionate about the future of data as we are, you’re in the right place!

  - block: markdown
    content:
      title: '👋 欢迎您'
      subtitle: ''
      text: '**浙江大学可持续数据智能与数据系统** 课题组成立于2023年，隶属于浙江大学数据库与数据智能实验室。我们专注于从算法和系统层面构建**快速、可靠、负责且弹性**的大数据智能计算解决方案。

      <p> 实验室现有硕博研究生十数人，成果长期一贯发表在相关领域的国际顶级学术会议/期刊，如SIGMOD、VLDB、ICDE、KDD、WWW、ICLR、ACL、CSUR、TKDE等。团队承担多项国家级攻关项目，并与国内头部企业有长期深厚的合作关系。<p/>'
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
        padding: ['300px', '0', '300px', '0']
      css_class:

  - block: collection
    content:
      title: 近期动态
      subtitle:
      text:
      count: 2
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
      title:
      subtitle:
      text: |
        {{% cta cta_link="./people/" cta_text="团队成员 →" %}}
    design:
      columns: '1'
---
