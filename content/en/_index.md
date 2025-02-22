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
      title: '👋 Hello'
      subtitle: ''
      text: 'Welcome to SuDIS the Sustainable Data Intelligence and Data Systems research group at Zhejiang University, where we hack on making data smarter and systems stronger. We explore modern architectures and algorithms to achieve **Rapid, Reliable, Responsible, and Resilient** solutions that tackle real-world problems. If you’re as passionate about the future of data as we are, you’re in the right place!'
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
      title: Latest News
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
      title:
      subtitle:
      text: |
        {{% cta cta_link="./people/" cta_text="Meet the team →" %}}
    design:
      columns: '1'
---
